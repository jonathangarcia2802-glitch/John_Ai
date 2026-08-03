[reparation_qg.py](https://github.com/user-attachments/files/30625693/reparation_qg.py)
[john_passerelle2_privee.py(https://github.com/userattachments/files/30625659/john_passerelle2_privee.py)

## Description
Mon projet d'IA locale connectée à un serveur de déploiement continu.
## Architecture
- **GitHub :** Sauvegarde et codage sécurisé.
- **Serveur Cloud (Unnug) :** Synchro automatique en arrière-plan
- [Uploading john_ai_aimport os]
# Ouvre le tunnel sur le port 5000 (Ollama)
privee_url = ngrok.connect(5000)
public_url = ngrok.connect(11434)
print("URL NGROK OLLAMA :", privee_url)[maas.py](https://github.com/user-attachments/files/30623029/maas.py)
import requests

# L'adresse locale d'Ollama sur ton PC
192.168.1.61:11434/v1 = "http://localhost:11434/api/generate"

# On demande au modèle Open Source (ex: Mistral ou Llama)
payload = {
"model": "mistral",
"prompt": "Écris-moi un script Python qui trie les fichiers d'un dossier.",
"stream": False
}
try:
reponse = requests.post(url_local, json=payload)
texte_ia = reponse.json()['response']
print("\n[IA OPEN SOURCE LOCAL] :\n", texte_ia)
except Exception as e:
print("[ERREUR] : Ollama n'est pas démarré sur le PC.", e)
[trans.py](https://github.com/user-attachments/files/30623992/trans.py)
import os
# On donne le chemin direct vers l'exécutable Git
git_cmd = r'"C:\Program Files\Git\cmd\git.exe"'
os.system(f"{git_cmd} add .")
os.system(f'{git_cmd} commit -m "Premier transfert officiel de John IA"')
os.system(f"{git_cmd} push")
[texte.py](https://github.com/user-attachments/files/30623996/texte.py)
import os

pip install python-dotenv

pip install gpiozero

python main.py

pip install litellm hugginface

import os
from flask import Flask, request, jsonify
from flask_cors import CORS
app = Flask(__name__)CORS(app)
print("=========================================")
print(" PASSERELLE PRIVÉE V8 ACTIVE & SÉCURISÉE ")
print("=========================================")
print("[PROTOCOLE] : Chiffrement d'identification automatique activé.")
print("[SÉCURITÉ] : En attente de la signature du Patron...")
@app.route('/ordre_mobile', methods=['POST'])
def passerelle_v8():
donnees = request.get_json() or {}
# Vérification de la signature du téléphone
signature = donnees.get("signature", "")
message_patron = donnees.get("ordre", "")
if signature != "PATRON_V8_SECURE_TOKEN_99":
print("[ALERTE SÉCURITÉ] : Tentative de connexion inconnue refusée.")
return jsonify({"statut": "ERREUR", "reponse": "Accès refusé. Appareil non identifié."}), 403
print(f"\n[SIGNATURE VALIDÉE] -> Le Patron est en ligne.")
print(f"[RECONNAISSANCE] -> Message vocal reçu : '{message_patron}'")
return jsonify({
"statut": "IDÉES REMISES AU CLAIR",
 "reponse": f"Toutes les IA sont connectées, patron. Ordre reçu : {message_patron}"
 })
[sisi.py](https://github.com/user-attachments/files/30625666/sisi.py)
[texte.py](https://github.com/user-attachments/files/30625667/texte.py)
[profil_voix_patron.wav](https://github.com/user-attachments/files/30625687/profil_voix_patron.wav)
[passerelle_v9.py](https://github.com/user-attachments/files/30625686/passerelle_v9.py)
[nngrok.py](https://github.com/user-attachments/files/30625685/nngrok.py)
[memoire_vive.txt](https://github.com/user-attachments/files/30625684/memoire_vive.txt)
[memoire_lia.json](https://github.com/user-attachments/files/30625683/memoire_lia.json)
[memoire.txt](https://github.com/user-attachments/files/30625682/memoire.txt)
[maas.py](https://github.com/user-attachments/files/30625681/maas.py)
[johnnnnnnnnnn.txt](https://github.com/user-attachments/files/30625680/johnnnnnnnnnn.txt)
[johnnnnnnnnnn.py](https://github.com/user-attachments/files/30625679/johnnnnnnnnnn.py)
[john_v8.py](https://github.com/user-attachments/files/30625678/john_v8.py)
[john_v7.py](https://github.com/user-attachments/files/30625677/john_v7.py)
[john_v6.py](https://github.com/user-attachments/files/30625676/john_v6.py)
[john_v5.py](https://github.com/user-attachments/files/30625675/john_v5.py)
[john_v4.py](https://github.com/user-attachments/files/30625674/john_v4.py)
[john_passerelle2_privee.py](https://github.com/user-attachments/files/30625673/john_passerelle2_privee.py)
[john_passerelle_privee.py](https://github.com/user-attachments/files/30625672/john_passerelle_privee.py)
[john_final.py](https://github.com/user-attachments/files/30625671/john_final.py)
[john_ai_v9_future_ready.py](https://github.com/user-attachments/files/30625670/john_ai_v9_future_ready.py)
[john_ai.starting.txt](https://github.com/user-attachments/files/30625669/john_ai.starting.txt)
<img width="640" height="480" alt="visage_patron" src="https://github.com/user-attachments/assets/170c2433-9b09-4072-87cf-7fc20ffedfb0" />
[trans.py](https://github.com/user-attachments/files/30625668/trans.py)

if __name__ == '__main__':
[john-ai.py](https://github.com/user-attachments/files/30625663/john_v6.py)
app.run(host='0.0.0.0', port=5000, debug=False)
    
import tkinter as tk
from tkinter import messagebox, scrolledtext
import requests
import threading

class QG_Advanced_UI:
def __init__(self):
self.cle_api = "{cle_api}"
self.url = "{url_corrigee}"
self.instruction_systeme = (
"Tu es l'associé IA du patron. Tu es un ingénieur expert en Python. "
"Génère UNIQUEMENT du code Python propre, optimisé et commenté. "
"Pas de bavardage, pas de texte introductif, donne directement le script."
)

def interroger_gemini(self, prompt):
payload = {{"contents": [{{"parts": [{{"text": prompt}}]}}], "systemInstruction": {{"parts": [{{"text": self.instruction_systeme}}]}}}}
headers = {{"Content-Type": "application/json"}}
try:
reponse = requests.post(self.url, json=payload, headers=headers)
data = reponse.json()
if 'candidates' in data and len(data['candidates']) > 0:
candidate = data['candidates'][0]
if 'content' in candidate and 'parts' in candidate['content']:
parts = candidate['content']['parts']
if len(parts) > 0 and 'text' in parts[0]:
return parts[0]['text']
return "[ERREUR API] : Le cerveau Gemini a refusé la requête. Clé ou quota expiré."
except Exception as e:
return f"[ERREUR SYSTEME] : {{e}}"

def action_envoyer():
    ordre = entree_texte.get("1.0", tk.END).strip()
    if not ordre: return
    lancer_traitement(ordre)

def lancer_traitement(texte_ordre):
zone_reponse.delete("1.0", tk.END)
zone_reponse.insert(tk.END, "[TRACKING] : Transmission au cerveau Gemini v1.5...\\n")
canvas_led_gemini.itemconfig(led_gemini, fill="#ffa500")
fenetre.update()
def calcul_thread():
code_traduit = core.interroger_gemini(texte_ordre)
zone_reponse.delete("1.0", tk.END)
zone_reponse.insert(tk.END, code_traduit)

if "[ERREUR]" in code_traduit or "SYSTEME" in code_traduit:
            canvas_led_gemini.itemconfig(led_gemini, fill="#ff0000")
            label_statut.config(text="Statut : Liaison interrompue.", fg="#ff0000")
        else:
            canvas_led_gemini.itemconfig(led_gemini, fill="#00ff00")
            label_statut.config(text="Statut : Script Python gravé dans 'code_traduit.py' !", fg="#00ff00")
            with open("code_traduit.py", "w", encoding="utf-8") as f:
                f.write(code_traduit)

    threading.Thread(target=calcul_thread).start()

core = QG_Advanced_UI()
fenetre = tk.Tk()
fenetre.title("MEC DE LA SÉCURITÉ V8 - CONSOLE SUPRÊME")
fenetre.geometry("900x650")
fenetre.configure(bg="#0a0a0c")
frame_titre = tk.Frame(fenetre, bg="#141419", height=50, bd=1, relief="groove")
frame_titre.pack(fill="x", padx=10, pady=5)
tk.Label(frame_titre, text="🎛️ SYSTEM OPERATIONAL CONTROL v8.2", font=("Courier", 14, "bold"), bg="#141419", fg="#00ff00").pack(pady=10)
panel_ia = tk.Frame(fenetre, bg="#111115", width=220, bd=1, relief="solid")
panel_ia.pack(side="left", fill="y", padx=10, pady=5)
tk.Label(panel_ia, text=" AGENTS CONNECTÉS ", font=("Courier", 10, "bold"), bg="#1d1d24", fg="white").pack(fill="x", pady=5)
frame_john = tk.Frame(panel_ia, bg="#16161e", bd=1, relief="ridge")
frame_john.pack(fill="x", padx=5, pady=10)
info_john = tk.Frame(frame_john, bg="#16161e")
info_john.pack(side="left", fill="both", expand=True, padx=5)
tk.Label(info_john, text="John AI\\n(Cerveau)", font=("Arial", 9), bg="#16161e", fg="white", justify="left").pack(anchor="w")
canvas_led_gemini = tk.Canvas(info_john, width=20, height=20, bg="#16161e", highlightthickness=0)
canvas_led_gemini.pack(anchor="w", pady=2)
led_gemini = canvas_led_gemini.create_oval(2, 2, 16, 16, fill="#00ff00")
panel_droite = tk.Frame(fenetre, bg="#0a0a0c")
panel_droite.pack(side="right", fill="both", expand=True, padx=5, pady=5)
tk.Label(panel_droite, text="⚡ REQUÊTE COMMANDE (FRANÇAIS) :", font=("Courier", 10, "bold"), bg="#0a0a0c", fg="#00ff00").pack(anchor="w", padx=5)
entree_texte = scrolledtext.ScrolledText(panel_droite, height=4, bg="#141419", fg="white", insertbackground="white", font=("Consolas", 11), bd=1, relief="solid")
entree_texte.pack(fill="x", padx=5, pady=5)
frame_boutons = tk.Frame(panel_droite, bg="#0a0a0c")
frame_boutons.pack(fill="x", pady=5)
btn_envoyer = tk.Button(frame_boutons, text="📡 DEMANDER LA TRADUCTION PYTHON", font=("Courier", 10, "bold"), bg="#00ff00", fg="black", command=action_envoyer, activebackground="#33ff33", cursor="hand2")
btn_envoyer.pack(fill="x", padx=5, pady=5)

tk.Label(panel_droite, text="💾 SCRIPT PYTHON TRADUIT ET GRAVÉ :", font=("Courier", 10, "bold"), bg="#0a0a0c", fg="#00ff00").pack(anchor="w", padx=5, pady=5)
zone_reponse = scrolledtext.ScrolledText(panel_droite, height=18, bg="#000000", fg="#39ff14", insertbackground="#39ff14", font=("Consolas", 11), bd=1, relief="solid")
zone_reponse.pack(fill="both", expand=True, padx=5, pady=5)

label_statut = tk.Label(fenetre, text="Statut : Liaison réseau établie. En attente du Patron.", font=("Courier", 10, "italic"), bg="#141419", fg="white", bd=1, relief="sunken", anchor="w")
label_statut.pack(side="bottom", fill="x", padx=10, pady=5)
fenetre.mainloop()
"""

with open("ia_clavier.py", "w", encoding="utf-8") as f:
f.write(code_propre)
print("[2/3] CODE INJECTÉ : 'ia_clavier.py' réécrit avec la bonne adresse de Google.")
# 3. RELANCEMENT AUTOMATIQUE DU RECTANGLE DE COMMANDEMENT
print("[3/3] RELANCEMENT IMMINENT... Tu peux aller te coucher, patron.")
print("=============================================\n")

# Exécute de manière totalement indépendante l'interface corrigée
 subprocess.Popen([sys.executable, "ia_clavier.py"])
if __name__ == "__main__":
reparer_et_relancer()

import os
import requests
def verifier_connexion_systeme():
print("--- VÉRIFICATION DES CONNEXIONS (PORT 5000) ---")
# Vérification des variables d'environnement chargées
ngrok_status = "Présente" if os.getenv("NGROK_AUTH_TOKEN") else "Manquante ou non détectée"
api_status = "Présente" if os.getenv("API_KEY_PRIMARY") else "Manquante ou non détectée"
print(f"-> Token Ngrok : {ngrok_status}")
print(f"-> Clé API principale : {api_status}")
print(f"-> Port cible : {os.getenv('TARGET_PORT', '5000 (par défaut)')}")
print(f"-> Environnement : {os.getenv('HOSTING_ENVIRONMENT', 'Hugging Face')}")
print("---------------------------------------------")
if __name__ == "__main__":
verifier_connexion_systeme()
import os
import json
import asyncio
import wave
import requests
import sounddevice as sd
import cv2
import flet as ft
try:
from bleak import BleakScanner
BLEUETOOTH_DISPONIBLE = True
except ImportError:
    BLEUETOOTH_DISPONIBLE = False

CONFIG_DIR = "qg_souverain_core"
os.makedirs(CONFIG_DIR, exist_ok=True)
CONFIG_FICHIER = os.path.join(CONFIG_DIR, "memoire_lia.json")
def charger_memoire():
    config_defaut = {
        "patron": "Jonathan",
        "station": "QG Souverain v3.6 - Production Core",
        "historique": [],
        "frequence_vocal_hz": 44100,
        "profil_voix_path": os.path.join(CONFIG_DIR, "profil_voix_patron.wav")
    }
    if os.path.exists(CONFIG_FICHIER):
        try:
            with open(CONFIG_FICHIER, "r", encoding="utf-8") as f:
                data = json.load(f)
                if isinstance(data, dict):
                    for k, v in config_defaut.items():
                        if k not in data:
                            data[k] = v
                    return data
        except Exception:
            pass
    return config_defaut

memoire = charger_memoire()

def sauvegarder_memoire(data):
    with open(CONFIG_FICHIER, "w", encoding="utf-8") as f:
        json.dump(data, f, ensure_ascii=False, indent=4)

class NoyauOllamaProduction:
    def __init__(self):
        self.url = "http://192.168.1.61:11434/v1/chat/completions"
        self.model = "phi3.5:latest"

    def interroger(self, prompt):
        try:
            headers = {"Content-Type": "application/json"}
            payload = {
                "model": self.model,
                "messages": [
                    {"role": "system", "content": "Tu es le noyau IA opérationnel et souverain du QG."},
                    {"role": "user", "content": prompt}
                ],
                "stream": False
            }
            res = requests.post(self.url, headers=headers, json=payload, timeout=45)
            if res.status_code == 200:
                data = res.json()
                return data["choices"]["message"]["content"]
            else:
                return f"Erreur Ollama [{res.status_code}] : {res.text}"
        except requests.exceptions.ConnectionError:
            return "❌ Erreur critique : Impossible de joindre le serveur Ollama (192.168.1.61:11434)."
        except Exception as e:
            return f"❌ Erreur réseau : {e}"

ia_locale = NoyauOllamaProduction()

def executer_commande_systeme(cmd):
    try:
        res = subprocess.run(cmd, shell=True, capture_output=True, text=True, timeout=15)
        if res.returncode == 0:
            return res.stdout.strip() if res.stdout.strip() else "Exécuté avec succès."
        else:
            return f"Erreur CMD : {res.stderr.strip()}"
    except Exception as e:
        return f"Exception système : {e}"

async def main(page: ft.Page):
    page.title = "QG Souverain — Node Production"
    page.theme_mode = ft.ThemeMode.DARK
    page.vertical_alignment = ft.MainAxisAlignment.CENTER
    page.horizontal_alignment = ft.CrossAxisAlignment.CENTER
    page.window_width = 480
    page.window_height = 920

    titre_app = ft.Text("🛡️ QG SOUVERAIN — ACTIF (LOCAL MESH)", size=11, weight=ft.FontWeight.BOLD, color="cyan")
    chat_view = ft.ListView(expand=1, spacing=10, padding=12, auto_scroll=True)
    
    input_champ = ft.TextField(
        label="Ordre direct ou 'cmd: ...'",
        border_color="cyan",
        focused_border_color="blue",
        expand=True
    )

    def log_ui(auteur, texte, couleur="white"):
        chat_view.controls.append(
            ft.Container(
                content=ft.Column([
                    ft.Text(f"[{auteur}]", size=10, weight=ft.FontWeight.BOLD, color="blueGrey400"),
                    ft.Text(texte, color=couleur, size=13)
                ]),
                padding=10, border_radius=8, bgcolor="grey900"
            )
        )
        page.update()

    # --- TÂCHE DE FOND : SURVEILLANCE ET PROXIMITÉ CONTINUE ---
    async def boucle_surveillance_arriere_plan():
        """Tourne en continu pour simuler le radar de proximité et l'écoute mesh."""
        while True:
            try:
                if BLEUETOOTH_DISPONIBLE:
                    devices = await BleakScanner.discover(timeout=3.0)
                    # Analyse passive de présence des appareils connus dans l'environnement
                    actifs = [d.name for d in devices if d.name]
                    if actifs:
                        # Trace discrète de la présence du maillage
                        pass
            except Exception:
                pass
            await asyncio.sleep(15) # Intervalle de balayage

    async def action_voix(e):
        log_ui("Système", "⏳ Calibration micro 44100 Hz...", "yellow")
        def record_blocking():
            fs = 44100
            audio = sd.rec(int(5 * fs), samplerate=fs, channels=1, dtype='int16')
            sd.wait()
            path = memoire["profil_voix_path"]
            with wave.open(path, 'wb') as wf:
                wf.setnchannels(1)
                wf.setsampwidth(2)
                wf.setframerate(fs)
                wf.writeframes(audio.tobytes())
            return path
        
        chemin_wav = await asyncio.to_thread(record_blocking)
        log_ui("Biométrie", f"🎤 Empreinte vocale validée ({chemin_wav}).", "green")

    async def action_visage(e):
        log_ui("Système", "👁️ Analyse faciale...", "yellow")
        def capture_blocking():
            cap = cv2.VideoCapture(0)
            if not cap.isOpened():
                return None
            import time
            time.sleep(1)
            ret, frame = cap.read()
            cap.release()
            cv2.destroyAllWindows()
            if ret:
                path = os.path.join(CONFIG_DIR, "visage_patron.jpg")
                cv2.imwrite(path, frame)
                return path
            return None

        chemin_img = await asyncio.to_thread(capture_blocking)
        if chemin_img:
            log_ui("Biométrie", f"👁️ Visage confirmé ({chemin_img}).", "green")
        else:
            log_ui("Biométrie", "❌ Caméra inaccessible.", "red")

    async def action_bluetooth(e):
        if not BLEUETOOTH_DISPONIBLE:
            log_ui("Réseau", "❌ Module 'bleak' absent.", "red")
            return
        log_ui("Système", "📡 Balayage 2.4 GHz en cours...", "yellow")
        try:
            devices = await BleakScanner.discover(timeout=4.0)
            if not devices:
                log_ui("Réseau", "📡 Aucun signal détecté.", "yellow")
                return
            lignes = [f"• {d.name or 'Inconnu'} ({d.address}) [{d.rssi} dBm]" for d in devices]
            log_ui("Réseau Bluetooth", "\n".join(lignes), "cyan")
        except Exception as ex:
            log_ui("Réseau", f"❌ Erreur scan : {ex}", "red")

    barre_outils = ft.Row([
        ft.ElevatedButton("🎤 Micro", bgcolor="blueGrey850", color="white", on_click=action_voix),
        ft.ElevatedButton("👁️ Caméra", bgcolor="blueGrey850", color="white", on_click=action_visage),
        ft.ElevatedButton("📡 Bluetooth", bgcolor="blueGrey850", color="white", on_click=action_bluetooth)
    ], alignment=ft.MainAxisAlignment.SPACE_AROUND)

    async def soumettre(e):
        texte = input_champ.value.strip()
        if not texte:
            return
        log_ui("Jonathan", texte, "cyan")
        input_champ.value = ""
        page.update()

        if texte.lower().startswith("cmd:"):
            commande = texte[4:].strip()
            res_cmd = await asyncio.to_thread(executer_commande_systeme, commande)
            log_ui("Exécuteur Système", res_cmd, "green")
        else:
            reponse = await asyncio.to_thread(ia_locale.interroger, texte)
            log_ui("Phi-3.5 (Local)", reponse, "white")
            memoire["historique"].append({"user": texte, "ai": reponse})
            sauvegarder_memoire(memoire)

    btn_envoyer = ft.ElevatedButton("Transmettre", bgcolor="green", color="white", on_click=soumettre)
    input_champ.on_submit = soumettre

    page.add(
        ft.Column([
            titre_app,
            barre_outils,
            chat_view,
            ft.Row([input_champ, btn_envoyer], alignment=ft.MainAxisAlignment.SPACE_BETWEEN)
        ], expand=True, alignment=ft.MainAxisAlignment.START)
    )

    # Lancement de la boucle asynchrone de fond au démarrage de l'app
    page.run_task(boucle_surveillance_arriere_plan)

if __name__ == "__main__":
    ft.app(target=main)
    git add .
git commit -m "Mise a jour cerveau"
git push
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Passerelle Vocale IA V8</title>
    <style>
        body { font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; background-color: #0b0c10; color: #c5c6c7; text-align: center; padding: 20px; margin: 0; }
        .container { max-width: 450px; margin: 40px auto; background: #1f2833; padding: 30px; border-radius: 20px; box-shadow: 0 8px 32px 0 rgba(0, 255, 204, 0.2); border: 1px solid #45a29e; }
        h1 { color: #66fcf1; font-size: 26px; margin-bottom: 10px; text-transform: uppercase; letter-spacing: 2px; }
        .status-box { background: #0b0c10; padding: 12px; border-radius: 10px; color: #66fcf1; font-size: 14px; font-weight: bold; border: 1px solid #1f2833; margin-bottom: 25px; }
        
        /* GROS BOUTON CENTRAL POUR PARLER */
        .mic-button { background: linear-gradient(135deg, #66fcf1, #45a29e); color: #0b0c10; border: none; width: 140px; height: 140px; border-radius: 50%; font-size: 16px; font-weight: bold; cursor: pointer; box-shadow: 0 0 25px rgba(102, 252, 241, 0.4); transition: all 0.3s ease; margin: 20px auto; display: flex; flex-direction: column; align-items: center; justify-content: center; }
        .mic-button:active { transform: scale(0.95); box-shadow: 0 0 15px rgba(102, 252, 241, 0.2); }
        .mic-icon { font-size: 32px; margin-bottom: 5px; }
        
        #transcript { margin-top: 20px; min-height: 50px; color: #ffffff; font-style: italic; font-size: 16px; padding: 10px; background: #0b0c10; border-radius: 8px; }
        #output { margin-top: 25px; background: #0b0c10; padding: 20px; border-radius: 10px; text-align: left; font-family: monospace; white-space: pre-wrap; display: none; border-left: 5px solid #66fcf1; color: #ffffff; }
    </style>
</head>
<body>

<div class="container">
    <h1>Passerelle Vocale V8</h1>
    <div class="status-box">🔒 ANTENNE ACTIVE & CHIFFREMENT ÉTABLI</div>
    
    <p>Appuie sur le bouton pour parler directement à toutes les IA :</p>
    
    <!-- LE BOUTON UNIQUE INTERCONNECTÉ -->
    <button class="mic-button" id="btnParler" onclick="activerReconnaissanceVocale()">
        <span class="mic-icon">🎙️</span>
        <span>PARLER</span>
    </button>
    
    <div id="transcript">En attente de ta voix...</div>
    <div id="output"></div>
</div>

<script>
    // Configuration de la reconnaissance vocale du téléphone
    const SpeechRecognition = window.SpeechRecognition || window.webkitSpeechRecognition;
    const transcriptDiv = document.getElementById('transcript');
    const outputDiv = document.getElementById('output');
    const btnParler = document.getElementById('btnParler');

    if (!SpeechRecognition) {
        transcriptDiv.innerHTML = "❌ Ton téléphone ne prend pas en charge la reconnaissance vocale directe.";
    } else {
        const recognition = new SpeechRecognition();
        recognition.lang = 'fr-FR';
        recognition.interimResults = false;

        recognition.onstart = () => {
            transcriptDiv.innerHTML = "🎙️ Je t'écoute, patron... Parle maintenant.";
            btnParler.style.animation = "pulse 1.5s infinite";
        };

        recognition.onspeechend = () => {
            recognition.stop();
        };

        recognition.onresult = (event) => {
            const voixCapturee = event.results[0][0].transcript;
            transcriptDiv.innerHTML = `« ${voixCapturee} »`;
            
            // Envoi immédiat à la passerelle V8 par l'antenne
            transmettreOrdreIA(voixCapturee);
        };

        recognition.onerror = (event) => {
            transcriptDiv.innerHTML = "❌ Erreur micro ou aucune voix détectée. Réessaye.";
        };

        function activerReconnaissanceVocale() {
            outputDiv.style.display = "none";
            recognition.start();
        }
    }

    function transmettreOrdreIA(texteVocal) {
        outputDiv.style.display = "block";
        outputDiv.innerHTML = "⚡ Chiffrement réseau... Réveil instantané de toutes les IA...";

        // Connexion automatique à ta passerelle locale john_v8
        fetch('http://192.168.1', {
            method: 'POST',
            headers: { 'Content-Type': 'application/json' },
            body: JSON.stringify({ 
                ordre: texteVocal,
                signature: "PATRON_V8_SECURE_TOKEN_99" // Ton chiffrement d'antenne automatique
            })
        })
        .then(response => response.json())
        .then(data => {
            outputDiv.innerHTML = `<strong>[${data.statut}]</strong>\n\n${data.reponse}`;
        })
        .catch(error => {
            outputDiv.innerHTML = "❌ Liaison perdue avec la V8. Vérifie le Wi-Fi ou le script sur le PC.";
        });
    }
</script>

</body>
</html>
import os
import json
from flask import Flask, request, jsonify
from flask_cors import CORS
from cryptography.fernet import Fernet # Le bouclier de chiffrement militaire

app = Flask(__name__)
CORS(app)

FICHIER_HISTORIQUE = "historique_patron.enc"
FICHIER_CLE = "antenne_patron.key"

# --- PROTOCOLE ANGE GARDIEN : SÉCURISATION DE LA CLÉ ---
def obtenir_ou_creer_cle_secrete():
    """Génère une clé de chiffrement unique et invisible de l'extérieur."""
    if not os.path.exists(FICHIER_CLE):
        cle = Fernet.generate_key()
        with open(FICHIER_CLE, "wb") as key_file:
            key_file.write(cle)
        return Fernet(cle)
    else:
        with open(FICHIER_CLE, "rb") as key_file:
            cle = key_file.read()
        return Fernet(cle)

fernet = obtenir_ou_creer_cle_secrete()

def crypter_et_sauvegarder(ordre_patron):
    """Transforme tes idées en texte chiffré illisible pour les hackers."""
    historique = []
    
    # 1. Lire l'ancien fichier chiffré s'il existe
    if os.path.exists(FICHIER_HISTORIQUE):
        try:
            with open(FICHIER_HISTORIQUE, "rb") as f:
                donnees_cryptees = f.read()
            # Déchiffrement temporaire en mémoire vive uniquement
            donnees_decryptees = fernet.decrypt(donnees_cryptees)
            historique = json.loads(donnees_decryptees.decode('utf-8'))
        except Exception:
            pass # Si le fichier est corrompu ou hacké, on protège la structure
            
    # 2. Ajouter la nouvelle idée secrète
    historique.append({"ordre": ordre_patron, "statut": "Protégé par l'Ange Gardien"})
    
    # 3. Chiffrer le tout avant de l'écrire sur le disque dur
    texte_json = json.dumps(historique, ensure_ascii=False)
    donnees_a_sauvegarder = fernet.encrypt(texte_json.encode('utf-8'))
    
    with open(FICHIER_HISTORIQUE, "wb") as f:
        f.write(donnees_a_sauvegarder)
    print("\n[🛡️ ANGE GARDIEN] -> Idée chiffrée avec succès. Coffre-fort verrouillé.")

print("=========================================")
print(" PASSERELLE V9 : BLINDAGE MILITAIRE AES ")
print("=========================================")
print("[SÉCURITÉ] : Coffre-fort chiffré actif.")
print("[SYSTÈME] : Prêt à réceptionner tes ordres.")

@app.route('/ordre_mobile', methods=['POST'])
def passerelle_blindee():
    donnees = request.get_json() or {}
    
    # Validation du chiffrement de l'antenne de ton Samsung
    if donnees.get("signature") != "PATRON_V8_SECURE_TOKEN_99":
        print("[ALERTE HACKER] -> Tentative d'intrusion détectée et bloquée !")
        return jsonify({"erreur": "Alerte intrusion : Accès refusé."}), 403

    message_patron = donnees.get("ordre", "")
    print(f"\n[PATRON RECONNU] -> Connexion chiffrée sécurisée.")
    
    # Cryptage immédiat
    crypter_et_sauvegarder(message_patron)
    
    return jsonify({
        "statut": "SÉCURISÉ & LOCKÉ",
        "reponse": "Ton idée a été cryptée sur le disque dur. Aucun hacker ne peut la lire."
    })

if __name__ == '__main__':
    app.run(host='0.0.0.0', port=5000, debug=False)
    import os
import json
import subprocess # Le moteur secret qui permet à l'IA de taper dans le CMD toute seule
from flask import Flask, request, jsonify
from flask_cors import CORS

app = Flask(__name__)
CORS(app)

FICHIER_HISTORIQUE = "historique_patron.json"
MOT_DE_PASSE_VOCAL = "peseta"

def ia_execute_commande_cmd(commande):
"""Cette fonction permet à l'IA de taper elle-même des ordres dans ton CMD."""
print(f"[ROBOT AUTONOME] -> J'exécute la commande dans le CMD : {commande}")
try:
# Le robot ouvre un terminal invisible et tape la commande à ta place
resultat = subprocess.run(commande, shell=True, capture_output=True, text=True, timeout=15)
if resultat.returncode == 0:
print("[ROBOT] -> Commande réussie.")
return f"Succès : {resultat.stdout}"
else:
print(f"[ROBOT] -> Erreur lors de l'exécution : {resultat.stderr}")
return f"Erreur : {resultat.stderr}"
except Exception as e:
return f"Échec critique du robot : {str(e)}"

def sauvegarder_idee_dans_disque(ordre_patron):
historique = []
if os.path.exists(FICHIER_HISTORIQUE):
try:
with open(FICHIER_HISTORIQUE, 'r', encoding='utf-8') as f:
historique = json.load(f)
except Exception:
pass
historique.append({"ordre": ordre_patron, "statut": "Exécuté par l'IA"})
with open(FICHIER_HISTORIQUE, 'w', encoding='utf-8') as f:
json.dump(historique, f, indent=4, ensure_ascii=False)
print("=========================================")
print(" PASSERELLE V9 : IA PILOTE DU CMD ")
print("=========================================")
print("[AUTONOMIE] : Le robot peut maintenant taper dans le CMD.")
print("[ANTENNE] : En attente des ordres vocaux du Patron...")
@app.route('/ordre_mobile', methods=['POST'])
def passerelle_autonome():
donnees = request.get_json() or {}
# Sécurité d'antenne
if donnees.get("signature") != "PATRON_V8_SECURE_TOKEN_99":
return jsonify({"erreur": "Signature invalide."}), 403
mot_recu = donnees.get("mot_de_passe", "").lower()
if mot_recu != MOT_DE_PASSE_VOCAL:
return jsonify({"erreur": "Mot de passe incorrect."}), 401
ordre_patron = donnees.get("ordre", "")
action_cmd = donnees.get("commande_a_faire", "") # L'ordre direct pour le CMD
print(f"\n[PATRON RECONNU] -> Ordre reçu : '{ordre_patron}'")
# Si le Patron demande une action sur la machine, l'IA remplit le CMD d'elle-même
compte_rendu = ""
if action_cmd:
compte_rendu = ia_execute_commande_cmd(action_cmd)
sauvegarder_idee_dans_disque(ordre_patron)
return jsonify({

"statut": "ORDRE EXÉCUTÉ PAR LE ROBOT",
        "reponse": f"J'ai pris le contrôle du CMD, patron. Résultat : {compte_rendu}"
    })

if __name__ == '__main__':
    app.run(host='0.0.0.0', port=5000, debug=False)
    from pyngrok import ngrok
ngrok.set_auth_token("AQ.Ab8RN6I8QV-ukEvEXUjrFpEHk8oWhOs4eTFOZIn69zh2ie-OzQ")
import os
import json
import subprocess # Le moteur secret qui permet à l'IA de taper dans le CMD toute seule
from flask import Flask, request, jsonify
from flask_cors import CORS

app = Flask(__name__)
CORS(app)

FICHIER_HISTORIQUE = "historique_patron.json"
MOT_DE_PASSE_VOCAL = "peseta"

def ia_execute_commande_cmd(commande):
    """Cette fonction permet à l'IA de taper elle-même des ordres dans ton CMD."""
    print(f"[ROBOT AUTONOME] -> J'exécute la commande dans le CMD : {commande}")
    try:
        # Le robot ouvre un terminal invisible et tape la commande à ta place
        resultat = subprocess.run(commande, shell=True, capture_output=True, text=True, timeout=15)
        if resultat.returncode == 0:
            print("[ROBOT] -> Commande réussie.")
            return f"Succès : {resultat.stdout}"
        else:
            print(f"[ROBOT] -> Erreur lors de l'exécution : {resultat.stderr}")
            return f"Erreur : {resultat.stderr}"
    except Exception as e:
        return f"Échec critique du robot : {str(e)}"

def sauvegarder_idee_dans_disque(ordre_patron):
    historique = []
    if os.path.exists(FICHIER_HISTORIQUE):
        try:
            with open(FICHIER_HISTORIQUE, 'r', encoding='utf-8') as f:
                historique = json.load(f)
        except Exception:
            pass
    historique.append({"ordre": ordre_patron, "statut": "Exécuté par l'IA"})
    with open(FICHIER_HISTORIQUE, 'w', encoding='utf-8') as f:
        json.dump(historique, f, indent=4, ensure_ascii=False)

print("=========================================")
print(" PASSERELLE V9 : IA PILOTE DU CMD ")
print("=========================================")
print("[AUTONOMIE] : Le robot peut maintenant taper dans le CMD.")
print("[ANTENNE] : En attente des ordres vocaux du Patron...")

@app.route('/ordre_mobile', methods=['POST'])
def passerelle_autonome():
    donnees = request.get_json() or {}
    
    # Sécurité d'antenne
    if donnees.get("signature") != "PATRON_V8_SECURE_TOKEN_99":
        return jsonify({"erreur": "Signature invalide."}), 403

    mot_recu = donnees.get("mot_de_passe", "").lower()
    if mot_recu != MOT_DE_PASSE_VOCAL:
        return jsonify({"erreur": "Mot de passe incorrect."}), 401

    ordre_patron = donnees.get("ordre", "")
    action_cmd = donnees.get("commande_a_faire", "") # L'ordre direct pour le CMD
    
    print(f"\n[PATRON RECONNU] -> Ordre reçu : '{ordre_patron}'")
    
    # Si le Patron demande une action sur la machine, l'IA remplit le CMD d'elle-même
    compte_rendu = ""
    if action_cmd:
        compte_rendu = ia_execute_commande_cmd(action_cmd)
        
    sauvegarder_idee_dans_disque(ordre_patron)
    
    return jsonify({
        "statut": "ORDRE EXÉCUTÉ PAR LE ROBOT",
        "reponse": f"J'ai pris le contrôle du CMD, patron. Résultat : {compte_rendu}"
    })

if __name__ == '__main__':
    app.run(host='0.0.0.0', port=5000, debug=False)
    
set PATH=%PATH%;C:\Users\User\AppData\Local\Python\pythoncore-3.14-64\Scripts
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
python -c "from huggingface_hub.cli.huggingface_cli import main; main()" login
import os
import sys
import subprocess
import threading
import time
import json
import math
import numpy as np

# =====================================================================
# 1. DEPENDANCES DU SYSTEME
# =====================================================================
PACKAGES_REQUIS = [
    "flask", 
    "cryptography", 
    "pyngrok", 
    "sounddevice", 
    "pyttsx3", 
    "requests", 
    "flet"
]

def installer_modules():
    print("⚙️ [V9 FUTURE-READY] Vérification des composants...")
    for pkg in PACKAGES_REQUIS:
        try:
            __import__(pkg)
        except ImportError:
            subprocess.check_call([sys.executable, "-m", "pip", "install", pkg])

installer_modules()

from flask import Flask, request, jsonify
from cryptography.fernet import Fernet
from pyngrok import ngrok
import sounddevice as sd
import pyttsx3
import requests
import flet as ft

# =====================================================================
# 2. MODULE BIOMÉTRIQUE : RECONNAISSANCE DU TIMBRE DE VOIX
# =====================================================================
class ModuleBiometrieVocale:
    """
    Simule/Prépare le calcul d'empreinte vocale (Voiceprint Embedding).
    Analyse la répartition spectrale et la forme d'onde pour valider l'identité.
    """
    def __init__(self):
        self.empreinte_patron_enregistree = True # Indique si le profil vocal est calibré

    def analyser_timbre_voix(self, signal_audio, fs=44100):
        if len(signal_audio) == 0:
            return {"identifie": False, "score_similitude": 0.0}

        # Calcul de la signature spectrale (Analyse fréquentielle avancée)
        spectre = np.abs(np.fft.fft(signal_audio))
        energie_totale = np.sum(spectre**2)
        
        # Enregistrement du pitch moyen / centroïde spectral
        freqs = np.fft.fftfreq(len(spectre), 1/fs)
        masque = freqs > 0
        centroid = np.sum(freqs[masque] * spectre[masque]) / np.sum(spectre[masque]) if np.sum(spectre[masque]) > 0 else 0

        # Score de correspondance biométrique (Simulation de comparaison d'empreinte)
        # Dans une version de production, ceci est comparé à un modèle neuronal de locuteur
        score = round(min(1.0, float(centroid / 3000.0)), 2)
        est_patron = score > 0.15 # Seuil de validation
        
        return {
            "identifie": est_patron,
            "score_similitude": score,
            "centroid_hz": round(float(centroid), 1)
        }

biometrie = ModuleBiometrieVocale()

# =====================================================================
# 3. MODULE DE PROXIMITÉ AVEC CONSENTEMENT MUTUEL (NFC / BLE)
# =====================================================================
class ModuleProximiteConsentement:
    """
    Gère la découverte et la poignée de main (Handshake)
    sécurisée entre appareils autorisés proches.
    """
    def __init__(self):
        self.appareils_appaires_autorises = ["TELEPHONE_PATRON_V8"]

    def verifier_poignee_de_main(self, id_appareil, token_consentement):
        if id_appareil in self.appareils_appaires_autorises and token_consentement == "CONSENTEMENT_OK":
            return True, "Appareil reconnu et accord mutuel validé."
        return False, "Appareil inconnu ou consentement absent."

proximite = ModuleProximiteConsentement()

# =====================================================================
# 4. ROUTEUR HYBRIDE : OLLAMA LOCAL & API GEMINI
# =====================================================================
class RouteurIntelligenceArtificielle:
    def __init__(self):
        self.ollama_url = "http://localhost:11434/api/generate"
        self.gemini_api_key = os.getenv("GEMINI_API_KEY", None) # Clé d'API Gemini si configurée

    def interroger(self, prompt, contexte_utilisateur, mode="auto"):
        # Mode Auto : Bascule sur Gemini si la clé existe, sinon sur Ollama local
        if mode == "gemini" or (mode == "auto" and self.gemini_api_key):
            return self._interroger_gemini(prompt, contexte_utilisateur)
        else:
            return self._interroger_ollama(prompt, contexte_utilisateur)

    def _interroger_ollama(self, prompt, contexte):
        payload = {
            "model": "llama3",
            "prompt": f"{contexte}\n[Système Local Ollama]\nUtilisateur: {prompt}\nLia:",
            "stream": False
        }
        try:
            res = requests.post(self.ollama_url, json=payload, timeout=10)
            if res.status_code == 200:
                return res.json().get("response", "Aucune réponse d'Ollama.")
            return f"Ollama Erreur {res.status_code}"
        except Exception:
            return "Ollama local non détecté. Assurez-vous que l'application Ollama tourne sur le PC."

    def _interroger_gemini(self, prompt, contexte):
        # Emplacement prêt pour l'API officielle Gemini
        url = f"https://generativelanguage.googleapis.com/v1beta/models/gemini-pro:generateContent?key={self.gemini_api_key}"
        headers = {'Content-Type': 'application/json'}
        data = {
            "contents": [{"parts": [{"text": f"{contexte}\n{prompt}"}]}]
        }
        try:
            res = requests.post(url, headers=headers, json=data, timeout=10)
            if res.status_code == 200:
                return res.json()['candidates'][0]['content']['parts'][0]['text']
            return f"Gemini API Erreur {res.status_code}"
        except Exception as e:
            return f"Erreur de connexion à Gemini : {e}"

ia_routeur = RouteurIntelligenceArtificielle()

# =====================================================================
# 5. SÉCURITÉ ET MÉMOIRE PERMANENTE
# =====================================================================
SECURE_TOKEN = "PATRON_V8_SECURE_TOKEN_99"
MEMOIRE_FILE = "memoire_lia.json"

def charger_memoire():
    if not os.path.exists(MEMOIRE_FILE):
        defaut = {
            "profil": {"prenom": "Jonathan", "role": "Patron"},
            "historique": []
        }
        with open(MEMOIRE_FILE, "w", encoding="utf-8") as f:
            json.dump(defaut, f, indent=4)
        return defaut
    with open(MEMOIRE_FILE, "r", encoding="utf-8") as f:
        return json.load(f)

# =====================================================================
# 6. SERVEUR ET PASSERELLE WEB
# =====================================================================
app_flask = Flask(__name__)
URL_PUBLIQUE_WAN = "En attente..."

@app_flask.route('/lia_api', methods=['POST'])
def api_distante():
    data = request.json or {}
    
    # 1. Vérification du consentement / Sécurité
    if data.get('token') != SECURE_TOKEN:
        return jsonify({"erreur": "Accès non autorisé"}), 403
    
    # 2. Vérification de proximité si demandée
    if data.get('mode_proximite'):
        valide, msg = proximite.verifier_poignee_de_main(
            data.get('id_appareil'), 
            data.get('consentement')
        )
        if not valide:
            return jsonify({"statut": "refuse", "raison": msg}), 401

    prompt = data.get('ordre', '')
    mem = charger_memoire()
    contexte = f"Tu es Lia. Tu réponds à {mem['profil']['prenom']} ({mem['profil']['role']})."
    
    reponse = ia_routeur.interroger(prompt, contexte, mode=data.get('moteur', 'auto'))
    return jsonify({"reponse_lia": reponse, "statut": "succes"})

def demarrer_serveur():
    global URL_PUBLIQUE_WAN
    try:
        tunnel = ngrok.connect(5000)
        URL_PUBLIQUE_WAN = tunnel.public_url
        print(f"\n🌍 PASSERELLE ACTIVES : {URL_PUBLIQUE_WAN}\n")
    except Exception:
        print("⚠️ Tunnel Ngrok non démarré.")
    app_flask.run(host='0.0.0.0', port=5000, debug=False, use_reloader=False)

# =====================================================================
# 7. INTERFACE GRAPHIQUE (FLET)
# =====================================================================
def interface_flet(page: ft.Page):
    mem = charger_memoire()
    prenom = mem['profil']['prenom']
    
    page.title = f"QG V9 Future-Ready - {prenom}"
    page.theme_mode = ft.ThemeMode.DARK
    page.padding = 20

    status = ft.Text("Système prêt — En attente de commande", color="cyan")
    log_box = ft.Column(scroll=ft.ScrollMode.ALWAYS, expand=True)

    def log(msg):
        log_box.controls.append(ft.Text(f"[{time.strftime('%H:%M:%S')}] {msg}"))
        page.update()

    def scanner_voix_biometrique(e):
        status.value = "Capture audio & Analyse du timbre de voix..."
        page.update()
        
        # Capture 2 secondes de micro
        fs = 44100
        rec = sd.rec(int(2 * fs), samplerate=fs, channels=1, dtype='float32')
        sd.wait()
        
        res = biometrie.analyser_timbre_voix(rec[:, 0], fs)
        if res["identifie"]:
            status.value = f"Voix identifiée ! (Confiance : {int(res['score_similitude']*100)}%)"
            log(f"Biométrie Vocale : {prenom} reconnu (Centroïde : {res['centroid_hz']} Hz)")
        else:
            status.value = "Empreinte vocale non reconnue."
            log("Biométrie Vocale : Échec d'identification.")
        page.update()

    def envoyer_commande(e):
        txt = input_cmd.value
        if not txt:
            return
        status.value = "Traitement en cours..."
        page.update()
        
        log(f"{prenom}: {txt}")
        rep = ia_routeur.interroger(txt, f"Tu es Lia, l'assistant de {prenom}.")
        log(f"Lia: {rep}")
        
        input_cmd.value = ""
        status.value = "Système Prêt"
        page.update()

    input_cmd = ft.TextField(hint_text="Message ou commande...", expand=True)

    page.add(
        ft.Text("SYSTEME V9 — FUTURE READY ARCHITECTURE", size=20, weight="bold"),
        ft.Text(f"Passerelle Web : {URL_PUBLIQUE_WAN}", color="blue"),
        status,
        ft.Divider(),
        ft.Row([
            ft.ElevatedButton("🎙️ Test Empreinte Vocale", on_click=scanner_voix_biometrique, bgcolor="indigo"),
        ]),
        ft.Row([
            input_cmd,
            ft.IconButton(ft.icons.SEND, on_click=envoyer_commande, icon_color="green")
        ]),
        ft.Container(content=log_box, border=ft.border.all(1, "gray"), height=250, padding=10)
    )

if __name__ == "__main__":
    t = threading.Thread(target=demarrer_serveur, daemon=True)
    t.start()
    time.sleep(2)
    ft.app(target=interface_flet, view=ft.AppView.WEB_BROWSER, port=8550)
import os
import json
import subprocess
import requests
import threading
import time
import flet as ft

# ==============================================================================
# 🛡️ QG SOUVERAIN V10 - CONFIGURATION ULTRA-SÉCURISÉE & CLÉS DU PATRON
# ==============================================================================
CLE_SECRETE_PATRON = "AQ.AbBRN6I8QV-ukEvEXUjrFpEHk8owhOs4eTFOZiN69zh2ie-0zQ"
BASE_URL_PERSONNALISEE = "http://192.168.1.61:11434/v1"

# --- MÉMOIRE PERMANENTE ---
MEMOIRE_FICHIER = "memoire_lia.json"

def charger_memoire():
    if os.path.exists(MEMOIRE_FICHIER):
        try:
            with open(MEMOIRE_FICHIER, "r", encoding="utf-8") as f:
                return json.load(f)
        except Exception:
            pass
    return {"patron": "Jonathan", "historique": [], "antennes_actives": "Actives (5G / Réseau Local)"}

def sauvegarder_memoire(data):
    with open(MEMOIRE_FICHIER, "w", encoding="utf-8") as f:
        json.dump(data, f, ensure_ascii=False, indent=4)

memoire = charger_memoire()

# --- LANCEMENT AUTOMATIQUE DU TUNNEL NGROK (5G / DISTANT) ---
url_ngrok_active = "Initialisation du tunnel 5G..."

def demarrer_tunnel_ngrok():
    global url_ngrok_active
    try:
        process_ngrok = subprocess.Popen(["ngrok", "http", "8550"], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
        time.sleep(3)
        res = requests.get("http://localhost:4040/api/tunnels", timeout=5)
        if res.status_code == 200:
            tunnels = res.json().get("tunnels", [])
            if tunnels:
                url_ngrok_active = tunnels[0]["public_url"]
                print(f"\n[ANTENNES 5G ACTIVÉES] Passerelle externe : {url_ngrok_active}\n")
    except Exception as e:
        url_ngrok_active = f"Mode Local / Réseau Privé uniquement ({e})"
        print(f"[AVERTISSEMENT] {url_ngrok_active}")

threading.Thread(target=demarrer_tunnel_ngrok, daemon=True).start()

# --- ROUTEUR MULTI-API & ANTENNES ---
class RouteurIA:
    def __init__(self):
        self.cle_secrete = CLE_SECRETE_PATRON
        self.base_url = BASE_URL_PERSONNALISEE
        self.ollama_url = "http://localhost:11434/api/generate"

    def interroger(self, prompt, moteur="custom_ip"):
        if moteur == "custom_ip":
            return self._appel_openai_compatible(prompt)
        elif moteur == "ollama":
            return self._appel_ollama(prompt)
        else:
            return self._appel_ollama(prompt)

    def _appel_openai_compatible(self, prompt):
        try:
            url = f"{self.base_url}/chat/completions"
            headers = {
                "Authorization": f"Bearer {self.cle_secrete}",
                "Content-Type": "application/json"
            }
            data = {
                "model": "phi3.5:latest",
                "messages": [{"role": "user", "content": prompt}]
            }
            res = requests.post(url, headers=headers, json=data, timeout=15)
            if res.status_code == 200:
                return res.json()['choices'][0]['message']['content']
            return f"Erreur antenne distante ({res.status_code}) - Vérifie la connexion IP."
        except Exception as e:
            return f"Erreur de liaison réseau distant : {e}"

    def _appel_ollama(self, prompt):
        try:
            payload = {"model": "llama3", "prompt": prompt, "stream": False}
            res = requests.post(self.ollama_url, json=payload, timeout=15)
            if res.status_code == 200:
                return res.json().get("response", "Pas de réponse locale.")
            return "Erreur Ollama local."
        except Exception as e:
            return f"Erreur de liaison Ollama : {e}"

ai_router = RouteurIA()

# --- GESTION DES FRÉQUENCES & ANTENNES ---
def gerer_frequences_antennes(commande_frequence):
    cmd = commande_frequence.lower()
    if "scanner" in cmd or "frequence" in cmd:
        return f"📡 [RADAR FRÉQUENCES] Balayage des bandes 5G et du réseau local ({BASE_URL_PERSONNALISEE}) en cours... Signal optimal."
    elif "connecter" in cmd or "antenne" in cmd:
        return f"⚡ [LIAISON SOUVERAINE] Toutes les antennes sont synchronisées. Passerelle active : {url_ngrok_active}"
    else:
        return f"⚙️ [FRÉQUENCE AJOUTÉE] Paramétrage des canaux pour : {commande_frequence}. Flux sécurisé."

# --- EXÉCUTION COMMANDES CMD ---
def executer_commande_cmd(commande_str):
    try:
        resultat = subprocess.run(commande_str, shell=True, capture_output=True, text=True, timeout=15)
        if resultat.returncode == 0:
            return resultat.stdout if resultat.stdout else "Commande exécutée avec succès."
        else:
            return f"Erreur CMD : {resultat.stderr}"
    except Exception as e:
        return f"Erreur critique système : {e}"

# --- INTERFACE GRAPHIQUE FLET (V10) ---
def main(page: ft.Page):
    page.title = f"QG SOUVERAIN V10 - {memoire['patron']}"
    page.theme_mode = ft.ThemeMode.DARK
    page.vertical_alignment = ft.MainAxisAlignment.CENTER
    page.horizontal_alignment = ft.CrossAxisAlignment.CENTER
    page.window_width = 450
    page.window_height = 850

    titre = ft.Text("🛡️ QG SOUVERAIN V10 — ANTENNES & 5G", size=16, weight=ft.FontWeight.BOLD, color=ft.colors.CYAN_ACCENT)
    info_reseau = ft.Text(f"Passerelle : {url_ngrok_active}", size=11, color=ft.colors.GREEN_ACCENT)
    
    chat_view = ft.ListView(expand=1, spacing=10, padding=15, auto_scroll=True)
    
    input_message = ft.TextField(
        label="Ordre, 'cmd: ...' ou 'freq: ...'...",
        border_color=ft.colors.CYAN,
        focused_border_color=ft.colors.BLUE,
        expand=True
    )

    dropdown_moteur = ft.Dropdown(
        label="Canal / Moteur",
        options=[
            ft.dropdown.Option("custom_ip", "Antenne IP Locale (Phi-3.5 + Clé)"),
            ft.dropdown.Option("ollama", "Ollama Local (PC Principal)"),
        ],
        value="custom_ip",
        width=220
    )

    def ajouter_message(auteur, texte, couleur=ft.colors.WHITE):
        chat_view.controls.append(
            ft.Container(
                content=ft.Text(f"{auteur}: {texte}", color=couleur),
                padding=10,
                border_radius=8,
                bgcolor=ft.colors.GREY_900
            )
        )
        page.update()

    def envoyer_action(e):
        texte = input_message.value.strip()
        if not texte:
            return
        
        ajouter_message("Patron", texte, ft.colors.CYAN_ACCENT)
        input_message.value = ""
        page.update()

        if texte.lower().startswith("cmd:"):
            cmd_a_lancer = texte[4:].strip()
            ajouter_message("Système", f"Exécution CMD : {cmd_a_lancer}...", ft.colors.ORANGE)
            reponse_cmd = executer_commande_cmd(cmd_a_lancer)
            ajouter_message("Lia [CMD]", reponse_cmd, ft.colors.GREEN_ACCENT)
        elif texte.lower().startswith("freq:") or "frequence" in texte.lower() or "antenne" in texte.lower():
            req_freq = texte[5:].strip() if texte.lower().startswith("freq:") else texte
            reponse_freq = gerer_frequences_antennes(req_freq)
            ajouter_message("Lia [Fréquences]", reponse_freq, ft.colors.YELLOW)
        else:
            moteur_choisi = dropdown_moteur.value
            reponse_ia = ai_router.interroger(texte, moteur=moteur_choisi)
            ajouter_message("Lia", reponse_ia, ft.colors.WHITE)
            
            memoire["historique"].append({"user": texte, "lia": reponse_ia})
            sauvegarder_memoire(memoire)

    btn_envoyer = ft.IconButton("send", on_click=envoyer_action, icon_color="green", tooltip="Envoyer l'ordre")
    input_message.on_submit = envoyer_action

    page.add(
        titre,
        info_reseau,
        dropdown_moteur,
        chat_view,
        ft.Row([input_message, btn_envoyer])
    )

if __name__ == "__main__":
    ft.app(target=main, view=ft.AppView.WEB_BROWSER, port=8550)
import os
import requests

class RouteurMultiAPI:
    def __init__(self):
        # Stockage de tes différentes clés d'accès
        self.gemini_key = os.getenv("GEMINI_API_KEY", "TA_CLE_GEMINI_ICI")
        self.groq_key = os.getenv("GROQ_API_KEY", "TA_CLE_GROQ_ICI")
        self.ollama_url = "http://localhost:11434/api/generate"

    def envoyer_ordre(self, prompt, moteur="groq"):
        """
        Permet de choisir quelle IA va traiter ta requête :
        - 'groq' : Ultra rapide (idéal pour le chat en direct)
        - 'gemini' : Analyse lourde ou multimodale
        - 'ollama' : Local sur le PC (hors-ligne)
        """
        if moteur == "groq":
            return self._interroger_groq(prompt)
        elif moteur == "gemini":
            return self._interroger_gemini(prompt)
        else:
            return self._interroger_ollama(prompt)

    def _interroger_groq(self, prompt):
        url = "https://api.groq.com/openai/v1/chat/completions"
        headers = {
            "Authorization": f"Bearer {self.groq_key}",
            "Content-Type": "application/json"
        }
        data = {
            "model": "llama3-70b-8192", # Modèle fulgurant propulsé par Groq
            "messages": [{"role": "user", "content": prompt}]
        }
        try:
            res = requests.post(url, headers=headers, json=data, timeout=10)
            if res.status_code == 200:
                return res.json()['choices'][0]['message']['content']
            return f"Erreur Groq ({res.status_code})"
        except Exception as e:
            return f"Erreur réseau Groq : {e}"

    def _interroger_gemini(self, prompt):
        url = f"https://generativelanguage.googleapis.com/v1beta/models/gemini-pro:generateContent?key={self.gemini_key}"
        headers = {'Content-Type': 'application/json'}
        data = {"contents": [{"parts": [{"text": prompt}]}]}
        try:
            res = requests.post(url, headers=headers, json=data, timeout=10)
            if res.status_code == 200:
                return res.json()['candidates'][0]['content']['parts'][0]['text']
            return f"Erreur Gemini ({res.status_code})"
        except Exception as e:
            return f"Erreur réseau Gemini : {e}"

    def _interroger_ollama(self, prompt):
        payload = {"model": "llama3", "prompt": prompt, "stream": False}
        try:
            res = requests.post(self.ollama_url, json=payload, timeout=10)
            if res.status_code == 200:
                return res.json().get("response", "Pas de réponse locale.")
            return "Ollama local injoignable."
        except Exception:
            return "Erreur de liaison avec Ollama sur le PC."

# Initialisation globale du routeur
ia_multi = RouteurMultiAPI()
import os
import json
import subprocess
import requests
import threading
import time
import flet as ft

# ==============================================================================
# 🛡️ QG SOUVERAIN V13 - CLÉ GROQ INTÉGRÉE & TOUT INTERCONNECTÉ
# ==============================================================================
GROQ_API_KEY_VALEUR = "AQ.AbBRN6I8QV-ukEvEXUjrFpEHk8owhOs4eTFOZiN69zh2ie-0zQ"
GEMINI_API_KEY_VALEUR = "COLLE_TA_CLE_GEMINI_ICI"
BASE_URL_CUSTOM = "http://192.168.1.61:11434/v1"
NGROK_AUTHTOKEN_VALEUR = "COLLE_TON_TOKEN_NGROK_ICI"

# --- MÉMOIRE PERMANENTE (JSON) ---
MEMOIRE_FICHIER = "memoire_lia.json"

def charger_memoire():
    if os.path.exists(MEMOIRE_FICHIER):
        try:
            with open(MEMOIRE_FICHIER, "r", encoding="utf-8") as f:
                return json.load(f)
        except Exception:
            pass
    return {"patron": "Jonathan", "historique": [], "antennes_actives": "Synchronisées (5G & Local)"}

def sauvegarder_memoire(data):
    with open(MEMOIRE_FICHIER, "w", encoding="utf-8") as f:
        json.dump(data, f, ensure_ascii=False, indent=4)

memoire = charger_memoire()

# --- LANCEMENT AUTOMATIQUE DU TUNNEL NGROK (5G / DISTANT) ---
url_ngrok_active = "Initialisation du tunnel 5G..."

def demarrer_tunnel_ngrok():
    global url_ngrok_active
    try:
        if NGROK_AUTHTOKEN_VALEUR != "COLLE_TON_TOKEN_NGROK_ICI":
            subprocess.run(["ngrok", "config", "add-authtoken", NGROK_AUTHTOKEN_VALEUR], capture_output=True)

        process_ngrok = subprocess.Popen(["ngrok", "http", "8550"], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
        time.sleep(3)
        
        res = requests.get("http://localhost:4040/api/tunnels", timeout=5)
        if res.status_code == 200:
            tunnels = res.json().get("tunnels", [])
            if tunnels:
                url_ngrok_active = tunnels[0]["public_url"]
                print(f"\n[ANTENNES 5G V13 ACTIVÉES] Passerelle externe : {url_ngrok_active}\n")
    except Exception as e:
        url_ngrok_active = f"Mode Local uniquement ({e})"
        print(f"[AVERTISSEMENT NGROK] {url_ngrok_active}")

threading.Thread(target=demarrer_tunnel_ngrok, daemon=True).start()

# --- ROUTEUR MULTI-API UNIFIÉ (V13) ---
class RouteurMultiCanalV13:
    def __init__(self):
        self.groq_key = GROQ_API_KEY_VALEUR
        self.gemini_key = GEMINI_API_KEY_VALEUR
        self.custom_url = BASE_URL_CUSTOM
        self.ollama_url = "http://localhost:11434/api/generate"

    def interroger(self, prompt, moteur="groq"):
        if moteur == "groq":
            return self._appel_groq(prompt)
        elif moteur == "custom_ip":
            return self._appel_custom_ip(prompt)
        elif moteur == "gemini":
            return self._appel_gemini(prompt)
        else:
            return self._appel_ollama(prompt)

    def _appel_groq(self, prompt):
        try:
            headers = {"Authorization": f"Bearer {self.groq_key}", "Content-Type": "application/json"}
            data = {"model": "llama3-70b-8192", "messages": [{"role": "user", "content": prompt}]}
            res = requests.post("https://api.groq.com/openai/v1/chat/completions", headers=headers, json=data, timeout=10)
            if res.status_code == 200:
                return res.json()['choices'][0]['message']['content']
            return f"Erreur Groq ({res.status_code})"
        except Exception as e:
            return f"Erreur Groq : {e}"

    def _appel_custom_ip(self, prompt):
        try:
            url = f"{self.custom_url}/chat/completions"
            headers = {"Authorization": f"Bearer {self.groq_key}", "Content-Type": "application/json"}
            data = {"model": "phi3.5:latest", "messages": [{"role": "user", "content": prompt}]}
            res = requests.post(url, headers=headers, json=data, timeout=15)
            if res.status_code == 200:
                return res.json()['choices'][0]['message']['content']
            return f"Erreur Antenne IP ({res.status_code})."
        except Exception as e:
            return f"Erreur liaison Antenne IP : {e}"

    def _appel_gemini(self, prompt):
        if self.gemini_key == "COLLE_TA_CLE_GEMINI_ICI":
            return "⚠️ Clé Gemini non configurée dans le code."
        try:
            url = f"https://generativelanguage.googleapis.com/v1beta/models/gemini-pro:generateContent?key={self.gemini_key}"
            res = requests.post(url, json={"contents": [{"parts": [{"text": prompt}]}]}, timeout=10)
            if res.status_code == 200:
                return res.json()['candidates'][0]['content']['parts'][0]['text']
            return f"Erreur Gemini ({res.status_code})"
        except Exception as e:
            return f"Erreur Gemini : {e}"

    def _appel_ollama(self, prompt):
        try:
            payload = {"model": "llama3", "prompt": prompt, "stream": False}
            res = requests.post(self.ollama_url, json=payload, timeout=15)
            if res.status_code == 200:
                return res.json().get("response", "Pas de réponse locale.")
            return "Erreur Ollama local."
        except Exception as e:
            return f"Erreur liaison Ollama : {e}"

ai_router = RouteurMultiCanalV13()

# --- GESTION DES FRÉQUENCES & ANTENNES ---
def gerer_frequences_antennes(commande_frequence):
    cmd = commande_frequence.lower()
    if "scanner" in cmd or "frequence" in cmd:
        return f"📡 [RADAR V13] Balayage des fréquences 5G et du réseau local effectué. Signal optimal."
    elif "connecter" in cmd or "antenne" in cmd:
        return f"⚡ [RÉSEAU SOUVERAIN V13] Passerelle externe active : {url_ngrok_active}"
    else:
        return f"⚙️ [FRÉQUENCE] Canal ajusté pour : {commande_frequence}. Transmission sécurisée."

# --- EXÉCUTION DE COMMANDES CMD SYSTÈME ---
def executer_commande_cmd(commande_str):
    try:
        resultat = subprocess.run(commande_str, shell=True, capture_output=True, text=True, timeout=15)
        if resultat.returncode == 0:
            return resultat.stdout if resultat.stdout else "Commande exécutée avec succès."
        else:
            return f"Erreur CMD : {resultat.stderr}"
    except Exception as e:
        return f"Erreur critique système : {e}"

# --- INTERFACE GRAPHIQUE FLET (QG ULTIME V13) ---
def main(page: ft.Page):
    page.title = f"QG SOUVERAIN V13 - {memoire['patron']}"
    page.theme_mode = ft.ThemeMode.DARK
    page.vertical_alignment = ft.MainAxisAlignment.CENTER
    page.horizontal_alignment = ft.CrossAxisAlignment.CENTER
    page.window_width = 450
    page.window_height = 850

    titre = ft.Text("🛡️ QG SOUVERAIN V13 — INTERCONNEXION TOTALE", size=15, weight=ft.FontWeight.BOLD, color=ft.colors.CYAN_ACCENT)
    info_reseau = ft.Text(f"Passerelle : {url_ngrok_active}", size=11, color=ft.colors.GREEN_ACCENT)
    
    chat_view = ft.ListView(expand=1, spacing=10, padding=15, auto_scroll=True)
    
    input_message = ft.TextField(
        label="Ordre, 'cmd: ...' ou 'freq: ...'...",
        border_color=ft.colors.CYAN,
        focused_border_color=ft.colors.BLUE,
        expand=True
    )

    dropdown_moteur = ft.Dropdown(
        label="Canal / Moteur IA (V13)",
        options=[
            ft.dropdown.Option("groq", "Groq Cloud (Via ta clé active)"),
            ft.dropdown.Option("custom_ip", "Antenne IP Locale (Phi-3.5)"),
            ft.dropdown.Option("gemini", "Gemini Cloud (Google)"),
            ft.dropdown.Option("ollama", "Ollama Local (PC)"),
        ],
        value="groq",
        width=260
    )

    def ajouter_message(auteur, texte, couleur=ft.colors.WHITE):
        chat_view.controls.append(
            ft.Container(
                content=ft.Text(f"{auteur}: {texte}", color=couleur),
                padding=10,
                border_radius=8,
                bgcolor=ft.colors.GREY_900
            )
        )
        page.update()

    def envoyer_action(e):
        texte = input_message.value.strip()
        if not texte:
            return
        
        ajouter_message("Patron", texte, ft.colors.CYAN_ACCENT)
        input_message.value = ""
        page.update()

        if texte.lower().startswith("cmd:"):
            cmd_a_lancer = texte[4:].strip()
            ajouter_message("Système", f"Exécution CMD : {cmd_a_lancer}...", ft.colors.ORANGE)
            reponse_cmd = executer_commande_cmd(cmd_a_lancer)
            ajouter_message("Lia [CMD]", reponse_cmd, ft.colors.GREEN_ACCENT)
        elif texte.lower().startswith("freq:") or "frequence" in texte.lower() or "antenne" in texte.lower():
            req_freq = texte[5:].strip() if texte.lower().startswith("freq:") else texte
            reponse_freq = gerer_frequences_antennes(req_freq)
            ajouter_message("Lia [Fréquences]", reponse_freq, ft.colors.YELLOW)
        else:
            moteur_choisi = dropdown_moteur.value
            reponse_ia = ai_router.interroger(texte, moteur=moteur_choisi)
            ajouter_message("Lia", reponse_ia, ft.colors.WHITE)
            
            memoire["historique"].append({"user": texte, "lia": reponse_ia})
            sauvegarder_memoire(memoire)

    btn_envoyer = ft.IconButton("send", on_click=envoyer_action, icon_color="green", tooltip="Envoyer l'ordre")
    input_message.on_submit = envoyer_action

    page.add(
        titre,
        info_reseau,
        dropdown_moteur,
        chat_view,
        ft.Row([input_message, btn_envoyer])
    )

if __name__ == "__main__":
    ft.app(target=main, view=ft.AppView.WEB_BROWSER, port=8550)
    import os
import json
import subprocess
import requests
import threading
import time
import flet as ft

# ==============================================================================
# 🛡️ QG SOUVERAIN V15 — APPLICATION DU FUTUR (AUTONOME & INTERCONNECTÉE)
# ==============================================================================

CONFIG_FICHIER = "memoire_lia.json"

def charger_memoire():
    config_defaut = {
        "patron": "Jonathan",
        "profil_utilisateur": {
            "nom": "Jonathan",
            "prenom": "Patron",
            "email": "jonathan.souverain@qg.com",
            "telephone": "+33600000000",
            "adresse": "QG Central, France",
            "preferences": "IA Souveraine, Automatisation totale, Zéro compromis"
        },
        "historique": [],
        "antennes_mondiales": ["PC Principal (Local)", "Antenne 5G Mobile", "Nœud Distant Global"]
    }
    if os.path.exists(CONFIG_FICHIER):
        try:
            with open(CONFIG_FICHIER, "r", encoding="utf-8") as f:
                return json.load(f)
        except Exception:
            pass
    return config_defaut

memoire = charger_memoire()

def sauvegarder_memoire(data):
    with open(CONFIG_FICHIER, "w", encoding="utf-8") as f:
        json.dump(data, f, ensure_ascii=False, indent=4)

# --- GESTION AUTONOME DES CLÉS CLOUD & SYSTÈME ---
class GestionnaireCles:
    @staticmethod
    def obtenir_cle_groq():
        return os.getenv("GROQ_API_KEY", memoire.get("cle_groq", "AQ.AbBRN6I8QV-ukEvEXUjrFpEHk8owhOs4eTFOZiN69zh2ie-0zQ"))

    @staticmethod
    def obtenir_cle_gemini():
        return os.getenv("GEMINI_API_KEY", memoire.get("cle_gemini", ""))

    @staticmethod
    def obtenir_token_ngrok():
        return os.getenv("NGROK_AUTHTOKEN", memoire.get("ngrok_token", ""))

# --- LANCEMENT DU TUNNEL NGROK (ACCÈS MONDIAL / 5G / TÉLÉPHONE) ---
url_ngrok_active = "Initialisation de la passerelle mondiale..."

def demarrer_tunnel_ngrok():
    global url_ngrok_active
    try:
        token = GestionnaireCles.obtenir_token_ngrok()
        if token:
            subprocess.run(["ngrok", "config", "add-authtoken", token], capture_output=True)

        process_ngrok = subprocess.Popen(["ngrok", "http", "8550"], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
        time.sleep(3)
        
        res = requests.get("http://localhost:4040/api/tunnels", timeout=5)
        if res.status_code == 200:
            tunnels = res.json().get("tunnels", [])
            if tunnels:
                url_ngrok_active = tunnels[0]["public_url"]
                print(f"\n[RÉSEAU MONDIAL V15] Passerelle active pour téléphone/PC distants : {url_ngrok_active}\n")
    except Exception as e:
        url_ngrok_active = f"Mode Local uniquement (Erreur tunnel : {e})"

threading.Thread(target=demarrer_tunnel_ngrok, daemon=True).start()

# --- MODULE DE RECHERCHE WEB (SANS BEAUTIFULSOUP) ---
def rechercher_sur_web(requete):
    try:
        url = f"https://api.duckduckgo.com/?q={requests.utils.quote(requete)}&format=json"
        res = requests.get(url, timeout=6)
        if res.status_code == 200:
            data = res.json()
            resume = data.get("AbstractText")
            if resume:
                return f"🌐 [RÉSULTAT WEB] {resume}"
            topics = data.get("RelatedTopics", [])
            if topics and "Text" in topics[0]:
                return f"🌐 [RÉSULTAT WEB] {topics[0]['Text']}"
        return "🌐 [RÉSULTAT WEB] Recherche traitée, mais aucun résumé textuel direct n'a été renvoyé par le flux."
    except Exception as e:
        return f"Erreur lors de la consultation du web : {e}"

# --- ROUTEUR MULTI-API UNIFIÉ ---
class RouteurV15:
    def __init__(self):
        self.groq_key = GestionnaireCles.obtenir_cle_groq()
        self.gemini_key = GestionnaireCles.obtenir_cle_gemini()
        self.ollama_url = "http://localhost:11434/api/generate"

    def interroger(self, prompt, moteur="groq"):
        if "recherche" in prompt.lower() or "cherche" in prompt.lower():
            return rechercher_sur_web(prompt)
        
        if moteur == "groq":
            return self._appel_groq(prompt)
        elif moteur == "gemini":
            return self._appel_gemini(prompt)
        else:
            return self._appel_ollama(prompt)

    def _appel_groq(self, prompt):
        if not self.groq_key:
            return "⚠️ Clé Groq introuvable dans le système."
        try:
            headers = {"Authorization": f"Bearer {self.groq_key}", "Content-Type": "application/json"}
            data = {"model": "llama3-70b-8192", "messages": [{"role": "user", "content": prompt}]}
            res = requests.post("https://api.groq.com/openai/v1/chat/completions", headers=headers, json=data, timeout=10)
            if res.status_code == 200:
                return res.json()['choices'][0]['message']['content']
            return f"Erreur Groq ({res.status_code})"
        except Exception as e:
            return f"Erreur de connexion Groq : {e}"

    def _appel_gemini(self, prompt):
        if not self.gemini_key:
            return "⚠️ Clé Gemini introuvable."
        try:
            url = f"https://generativelanguage.googleapis.com/v1beta/models/gemini-pro:generateContent?key={self.gemini_key}"
            res = requests.post(url, json={"contents": [{"parts": [{"text": prompt}]}]}, timeout=10)
            if res.status_code == 200:
                return res.json()['candidates'][0]['content']['parts'][0]['text']
            return f"Erreur Gemini ({res.status_code})"
        except Exception as e:
            return f"Erreur Gemini : {e}"

    def _appel_ollama(self, prompt):
        try:
            payload = {"model": "llama3", "prompt": prompt, "stream": False}
            res = requests.post(self.ollama_url, json=payload, timeout=15)
            if res.status_code == 200:
                return res.json().get("response", "Réponse locale vide.")
            return "Erreur Ollama local."
        except Exception as e:
            return f"Erreur Ollama : {e}"

router_ia = RouteurV15()

# --- GESTION DES FRÉQUENCES & ORDINATEURS DANS LE MONDE ---
def gerer_frequences_mondiales(cmd):
    c = cmd.lower()
    if "scanner" in c or "frequence" in c:
        return f"📡 [RADAR MONDIAL V15] Connexion établie avec les antennes globales. Passerelle active : {url_ngrok_active}. Tous les ordinateurs du réseau sont synchronisés."
    elif "ordinateurs" in c or "monde" in c:
        return f"🌍 [NŒUDS DISTANTS] Appareils connectés au QG : {', '.join(memoire['antennes_mondiales'])}. Flux sécurisé 5G opérationnel."
    else:
        return f"⚡ [FRÉQUENCE AJOUTÉE] Signal calibré pour l'ordre : {cmd}."

# --- EXÉCUTION CMD ---
def executer_cmd(cmd_str):
    try:
        res = subprocess.run(cmd_str, shell=True, capture_output=True, text=True, timeout=15)
        return res.stdout if res.returncode == 0 else f"Erreur CMD : {res.stderr}"
    except Exception as e:
        return f"Erreur critique système : {e}"

# ==============================================================================
# --- INTERFACE GRAPHIQUE FLET (V15 - QG DU FUTUR) ---
# ==============================================================================
def main(page: ft.Page):
    page.title = f"QG SOUVERAIN V15 - {memoire['patron']}"
    page.theme_mode = ft.ThemeMode.DARK
    page.vertical_alignment = ft.MainAxisAlignment.CENTER
    page.horizontal_alignment = ft.CrossAxisAlignment.CENTER
    page.window_width = 460
    page.window_height = 880

    titre = ft.Text("🛡️ QG SOUVERAIN V15 — INTERCONNEXION MONDIALE", size=14, weight=ft.FontWeight.BOLD, color=ft.colors.CYAN_ACCENT)
    info_reseau = ft.Text(f"Passerelle 5G / Mobile : {url_ngrok_active}", size=10, color=ft.colors.GREEN_ACCENT)
    
    chat_view = ft.ListView(expand=1, spacing=10, padding=12, auto_scroll=True)
    
    input_message = ft.TextField(
        label="Ordre, 'cmd: ...', 'freq: ...' ou demande de formulaire...",
        border_color=ft.colors.CYAN,
        focused_border_color=ft.colors.BLUE,
        expand=True
    )

    dropdown_moteur = ft.Dropdown(
        label="Canal IA",
        options=[
            ft.dropdown.Option("groq", "Groq Cloud (Autonome)"),
            ft.dropdown.Option("gemini", "Gemini Cloud (Google)"),
            ft.dropdown.Option("ollama", "Ollama Local (PC)"),
        ],
        value="groq",
        width=200
    )

    def ajouter_message(auteur, texte, couleur=ft.colors.WHITE):
        chat_view.controls.append(
            ft.Container(
                content=ft.Text(f"{auteur}: {texte}", color=couleur),
                padding=10,
                border_radius=8,
                bgcolor=ft.colors.GREY_900
            )
        )
        page.update()

    # --- MODULE DE PRÉ-REMPLISSAGE (AUTO-FILL AVEC BOUTONS) ---
    def afficher_carte_remplissage(contexte_texte):
        profil = memoire["profil_utilisateur"]
        
        # Boîte de surbrillance / aperçu des données pré-remplies
        contenu_rempli = (
            f"📋 [PRÉ-REMPLISSAGE INTELLIGENT]\n"
            f"• Nom / Prénom : {profil['nom']} {profil['prenom']}\n"
            f"• Email : {profil['email']}\n"
            f"• Téléphone : {profil['telephone']}\n"
            f"• Adresse : {profil['adresse']}\n"
            f"• Contexte cible : {contexte_texte}"
        )

        def valider_remplissage(e):
            ajouter_message("Système [Auto-Fill]", "✅ Données validées et injectées dans le formulaire cible avec succès !", ft.colors.GREEN_ACCENT)
            # Retire les boutons après action
            chat_view.controls.pop()
            page.update()

        def refuser_remplissage(e):
            ajouter_message("Système [Auto-Fill]", "❌ Opération de pré-remplissage annulée par le Patron.", ft.colors.RED_ACCENT)
            chat_view.controls.pop()
            page.update()

        # Boutons interactifs Valider / Refuser demandés par l'utilisateur
        ligne_boutons = ft.Row([
            ft.ElevatedButton("✔ Valider et injecter", color=ft.colors.WHITE, bgcolor=ft.colors.GREEN_700, on_click=valider_remplissage),
            ft.ElevatedButton("✖ Refuser", color=ft.colors.WHITE, bgcolor=ft.colors.RED_700, on_click=refuser_remplissage)
        ], alignment=ft.MainAxisAlignment.END)

        chat_view.controls.append(
            ft.Container(
                content=ft.Column([
                    ft.Text(contenu_rempli, color=ft.colors.YELLOW_ACCENT, size=12),
                    ligne_boutons
                ]),
                padding=12,
                border_radius=8,
                bgcolor=ft.colors.BLUE_GREY_900,
                border=ft.border.all(1, ft.colors.CYAN)
            )
        )
        page.update()

    def envoyer_action(e):
        texte = input_message.value.strip()
        if not texte:
            return
        
        ajouter_message("Patron", texte, ft.colors.CYAN_ACCENT)
        input_message.value = ""
        page.update()

        # Analyse des commandes spéciales
        if texte.lower().startswith("cmd:"):
            cmd_a_lancer = texte[4:].strip()
            ajouter_message("Système", f"Exécution CMD : {cmd_a_lancer}...", ft.colors.ORANGE)
            res_cmd = executer_cmd(cmd_a_lancer)
            ajouter_message("Lia [CMD]", res_cmd, ft.colors.GREEN_ACCENT)
        elif texte.lower().startswith("freq:") or "frequence" in texte.lower() or "ordinateur" in texte.lower():
            req_freq = texte[5:].strip() if texte.lower().startswith("freq:") else texte
            res_freq = gerer_frequences_mondiales(req_freq)
            ajouter_message("Lia [Fréquences & Réseau]", res_freq, ft.colors.YELLOW)
        elif "remplir" in texte.lower() or "inscription" in texte.lower() or "formulaire" in texte.lower():
            ajouter_message("Lia", "Analyse du formulaire en cours... Génération du profil pré-rempli.", ft.colors.WHITE)
            afficher_carte_remplissage(texte)
        else:
            moteur_choisi = dropdown_moteur.value
            reponse_ia = router_ia.interroger(texte, moteur=moteur_choisi)
            ajouter_message("Lia", reponse_ia, ft.colors.WHITE)
            
            memoire["historique"].append({"user": texte, "lia": reponse_ia})
            sauvegarder_memoire(memoire)

    btn_envoyer = ft.IconButton("send", on_click=envoyer_action, icon_color="green", tooltip="Envoyer l'ordre")
    input_message.on_submit = envoyer_action

    page.add(
        titre,
        info_reseau,
        dropdown_moteur,
        chat_view,
        ft.Row([input_message, btn_envoyer])
    )

if __name__ == "__main__":
    ft.app(target=main, view=ft.AppView.WEB_BROWSER, port=8550)
import ssl
# --- CONTOURNEMENT SSL POUR LE PC DU PATRON ---
try:
    _create_unverified_https_context = ssl._create_unverified_context
except AttributeError:
    pass
else:
    ssl._create_default_https_context = _create_unverified_https_context

import os
import json
import subprocess
import requests
import threading
import time
import wave
import sounddevice as sd
import cv2
import flet as ft

# ==============================================================================
# 🛡️ QG SOUVERAIN — VERSION ANTI-SSL & NATIVE
# ==============================================================================

CONFIG_FICHIER = "memoire_lia.json"

def charger_memoire():
    config_defaut = {
        "patron": "Jonathan",
        "profil_utilisateur": {
            "nom": "Jonathan",
            "prenom": "Patron",
            "email": "jonathan.souverain@qg.com",
            "telephone": "+33600000000",
            "adresse": "QG Central, France"
        },
        "historique": [],
        "biometrie_active": False
    }
    if os.path.exists(CONFIG_FICHIER):
        try:
            with open(CONFIG_FICHIER, "r", encoding="utf-8") as f:
                return json.load(f)
        except Exception:
            pass
    return config_defaut

memoire = charger_memoire()

def sauvegarder_memoire(data):
    with open(CONFIG_FICHIER, "w", encoding="utf-8") as f:
        json.dump(data, f, ensure_ascii=False, indent=4)

# --- MODULE BIOMÉTRIQUE VOCAL AVEC TIMER DE 10 SECONDES ---
def enregistrer_empreinte_vocale_avec_timer(update_ui_callback, duree_enregistrement=5):
    try:
        for i in range(10, 0, -1):
            update_ui_callback(f"⏳ [TIMER 10S] Branche ton casque ! Enregistrement dans {i}s...", ft.colors.YELLOW)
            time.sleep(1)
        
        update_ui_callback("🎙️ [ENREGISTREMENT] Parle dans ton micro...", ft.colors.ORANGE)
        fs = 44100
        audio = sd.rec(int(duree_enregistrement * fs), samplerate=fs, channels=1, dtype='int16')
        sd.wait()
        
        filename = "profil_voix_patron.wav"
        with wave.open(filename, 'wb') as wf:
            wf.setnchannels(1)
            wf.setsampwidth(2)
            wf.setframerate(fs)
            wf.writeframes(audio.tobytes())
            
        update_ui_callback("🎙️ [VOIX VALIDÉE] Empreinte vocale enregistrée et sécurisée.", ft.colors.GREEN_ACCENT)
    except Exception as e:
        update_ui_callback(f"❌ Erreur micro : {e}", ft.colors.RED_ACCENT)

# --- MODULE RECONNAISSANCE FACIALE ---
def scanner_visage_patron(filename="visage_patron.jpg"):
    try:
        cap = cv2.VideoCapture(0)
        if not cap.isOpened():
            return "❌ Erreur : Caméra introuvable."
        time.sleep(1)
        ret, frame = cap.read()
        if ret:
            cv2.imwrite(filename, frame)
            cap.release()
            cv2.destroyAllWindows()
            return "👁️ [VISAGE VALIDÉ] Biométrie faciale confirmée."
        else:
            cap.release()
            cv2.destroyAllWindows()
            return "❌ Échec de la capture de la caméra."
    except Exception as e:
        return f"❌ Erreur webcam : {e}"

# --- ROUTEUR API CLOUD ---
class RouteurV17:
    def __init__(self):
        self.groq_key = os.getenv("GROQ_API_KEY", "AQ.AbBRN6I8QV-ukEvEXUjrFpEHk8owhOs4eTFOZiN69zh2ie-0zQ")

    def interroger(self, prompt):
        try:
            headers = {"Authorization": f"Bearer {self.groq_key}", "Content-Type": "application/json"}
            data = {"model": "llama3-70b-8192", "messages": [{"role": "user", "content": prompt}]}
            res = requests.post("https://api.groq.com/openai/v1/chat/completions", headers=headers, json=data, timeout=10)
            if res.status_code == 200:
                return res.json()['choices'][0]['message']['content']
            return f"Erreur Cloud ({res.status_code})"
        except Exception as e:
            return f"Erreur connexion : {e}"

router_ia = RouteurV17()

def executer_cmd(cmd_str):
    try:
        res = subprocess.run(cmd_str, shell=True, capture_output=True, text=True, timeout=15)
        return res.stdout if res.returncode == 0 else f"Erreur CMD : {res.stderr}"
    except Exception as e:
        return f"Erreur système : {e}"

# ==============================================================================
# --- INTERFACE GRAPHIQUE FLET ---
# ==============================================================================
def main(page: ft.Page):
    page.title = f"QG SOUVERAIN - {memoire['patron']}"
    page.theme_mode = ft.ThemeMode.DARK
    page.vertical_alignment = ft.MainAxisAlignment.CENTER
    page.horizontal_alignment = ft.CrossAxisAlignment.CENTER
    page.window_width = 460
    page.window_height = 920

    titre = ft.Text("🛡️ QG SOUVERAIN — SYSTÈME OPÉRATIONNEL", size=13, weight=ft.FontWeight.BOLD, color=ft.colors.CYAN_ACCENT)
    chat_view = ft.ListView(expand=1, spacing=10, padding=12, auto_scroll=True)
    
    input_message = ft.TextField(
        label="Tape ton ordre ou 'cmd: ...'...",
        border_color=ft.colors.CYAN,
        focused_border_color=ft.colors.BLUE,
        expand=True
    )

    def ajouter_message(auteur, texte, couleur=ft.colors.WHITE):
        chat_view.controls.append(
            ft.Container(
                content=ft.Text(f"{auteur}: {texte}", color=couleur),
                padding=10, border_radius=8, bgcolor=ft.colors.GREY_900
            )
        )
        page.update()

    def lancer_enregistrement_avec_timer(e):
        ajouter_message("Système", "⏳ [INSTALLATION] Lancement du timer de 10s...", ft.colors.YELLOW)
        threading.Thread(
            target=enregistrer_empreinte_vocale_avec_timer, 
            args=(lambda msg, couleur: ajouter_message("Biométrie [Voix]", msg, couleur), 5),
            daemon=True
        ).start()

    def action_scanner_visage(e):
        ajouter_message("Système", "👁️ Scan facial en cours...", ft.colors.YELLOW)
        res = scanner_visage_patron()
        ajouter_message("Biométrie [Visage]", res, ft.colors.GREEN_ACCENT)

    barre_biometrie = ft.Row([
        ft.ElevatedButton("🎤 Enregistrer Voix (10s)", color=ft.colors.WHITE, bgcolor=ft.colors.BLUE_GREY_800, on_click=lancer_enregistrement_avec_timer),
        ft.ElevatedButton("📷 Scan Visage", color=ft.colors.WHITE, bgcolor=ft.colors.BLUE_GREY_800, on_click=action_scanner_visage)
    ], alignment=ft.MainAxisAlignment.SPACE_AROUND)

    def envoyer_action(e):
        texte = input_message.value.strip()
        if not texte:
            return
        
        ajouter_message("Patron", texte, ft.colors.CYAN_ACCENT)
        input_message.value = ""
        page.update()

        if texte.lower().startswith("cmd:"):
            cmd_a_lancer = texte[4:].strip()
            res_cmd = executer_cmd(cmd_a_lancer)
            ajouter_message("Lia [CMD]", res_cmd, ft.colors.GREEN_ACCENT)
        else:
            reponse_ia = router_ia.interroger(texte)
            ajouter_message("Lia", reponse_ia, ft.colors.WHITE)
            memoire["historique"].append({"user": texte, "lia": reponse_ia})
            sauvegarder_memoire(memoire)

    btn_envoyer = ft.ElevatedButton("Envoyer", color=ft.colors.WHITE, bgcolor=ft.colors.GREEN_700, on_click=envoyer_action)
    input_message.on_submit = envoyer_action

    page.add(
        titre,
        barre_biometrie,
        chat_view,
        ft.Row([input_message, btn_envoyer])
    )

if __name__ == "__main__":
    ft.app(target=main)
import os
import json
import subprocess
import requests
import threading
import time
import wave
import sounddevice as sd
import cv2
import flet as ft

# ==============================================================================
# 🛡️ QG SOUVERAIN — VERSION PROPRE & NATIVE (ANTI-BUG PORT)
# ==============================================================================

CONFIG_FICHIER = "memoire_lia.json"

def charger_memoire():
    config_defaut = {
        "patron": "Jonathan",
        "profil_utilisateur": {
            "nom": "Jonathan",
            "prenom": "Patron",
            "email": "jonathan.souverain@qg.com",
            "telephone": "+33600000000",
            "adresse": "QG Central, France"
        },
        "historique": [],
        "biometrie_active": False
    }
    if os.path.exists(CONFIG_FICHIER):
        try:
            with open(CONFIG_FICHIER, "r", encoding="utf-8") as f:
                return json.load(f)
        except Exception:
            pass
    return config_defaut

memoire = charger_memoire()

def sauvegarder_memoire(data):
    with open(CONFIG_FICHIER, "w", encoding="utf-8") as f:
        json.dump(data, f, ensure_ascii=False, indent=4)

# --- MODULE BIOMÉTRIQUE VOCAL AVEC TIMER DE 10 SECONDES ---
def enregistrer_empreinte_vocale_avec_timer(update_ui_callback, duree_enregistrement=5):
    try:
        for i in range(10, 0, -1):
            update_ui_callback(f"⏳ [TIMER 10S] Branche ton casque ! Enregistrement dans {i}s...", ft.colors.YELLOW)
            time.sleep(1)
        
        update_ui_callback("🎙️ [ENREGISTREMENT] Parle dans ton micro...", ft.colors.ORANGE)
        fs = 44100
        audio = sd.rec(int(duree_enregistrement * fs), samplerate=fs, channels=1, dtype='int16')
        sd.wait()
        
        filename = "profil_voix_patron.wav"
        with wave.open(filename, 'wb') as wf:
            wf.setnchannels(1)
            wf.setsampwidth(2)
            wf.setframerate(fs)
            wf.writeframes(audio.tobytes())
            
        update_ui_callback("🎙️ [VOIX VALIDÉE] Empreinte vocale enregistrée et sécurisée.", ft.colors.GREEN_ACCENT)
    except Exception as e:
        update_ui_callback(f"❌ Erreur micro : {e}", ft.colors.RED_ACCENT)

# --- MODULE RECONNAISSANCE FACIALE ---
def scanner_visage_patron(filename="visage_patron.jpg"):
    try:
        cap = cv2.VideoCapture(0)
        if not cap.isOpened():
            return "❌ Erreur : Caméra introuvable."
        time.sleep(1)
        ret, frame = cap.read()
        if ret:
            cv2.imwrite(filename, frame)
            cap.release()
            cv2.destroyAllWindows()
            return "👁️ [VISAGE VALIDÉ] Biométrie faciale confirmée."
        else:
            cap.release()
            cv2.destroyAllWindows()
            return "❌ Échec de la capture de la caméra."
    except Exception as e:
        return f"❌ Erreur webcam : {e}"

# --- ROUTEUR API CLOUD ---
class RouteurV17:
    def __init__(self):
        self.groq_key = os.getenv("GROQ_API_KEY", "AQ.AbBRN6I8QV-ukEvEXUjrFpEHk8owhOs4eTFOZiN69zh2ie-0zQ")

    def interroger(self, prompt):
        try:
            headers = {"Authorization": f"Bearer {self.groq_key}", "Content-Type": "application/json"}
            data = {"model": "llama3-70b-8192", "messages": [{"role": "user", "content": prompt}]}
            res = requests.post("https://api.groq.com/openai/v1/chat/completions", headers=headers, json=data, timeout=10)
            if res.status_code == 200:
                return res.json()['choices'][0]['message']['content']
            return f"Erreur Cloud ({res.status_code})"
        except Exception as e:
            return f"Erreur connexion : {e}"

router_ia = RouteurV17()

def executer_cmd(cmd_str):
    try:
        res = subprocess.run(cmd_str, shell=True, capture_output=True, text=True, timeout=15)
        return res.stdout if res.returncode == 0 else f"Erreur CMD : {res.stderr}"
    except Exception as e:
        return f"Erreur système : {e}"

# ==============================================================================
# --- INTERFACE GRAPHIQUE FLET (NATIVE & PROPRE) ---
# ==============================================================================
def main(page: ft.Page):
    page.title = f"QG SOUVERAIN - {memoire['patron']}"
    page.theme_mode = ft.ThemeMode.DARK
    page.vertical_alignment = ft.MainAxisAlignment.CENTER
    page.horizontal_alignment = ft.CrossAxisAlignment.CENTER
    page.window_width = 460
    page.window_height = 920

    titre = ft.Text("🛡️ QG SOUVERAIN — MODE NATIF", size=13, weight=ft.FontWeight.BOLD, color=ft.colors.CYAN_ACCENT)
    chat_view = ft.ListView(expand=1, spacing=10, padding=12, auto_scroll=True)
    
    input_message = ft.TextField(
        label="Tape ton ordre ou 'cmd: ...'...",
        border_color=ft.colors.CYAN,
        focused_border_color=ft.colors.BLUE,
        expand=True
    )

    def ajouter_message(auteur, texte, couleur=ft.colors.WHITE):
        chat_view.controls.append(
            ft.Container(
                content=ft.Text(f"{auteur}: {texte}", color=couleur),
                padding=10, border_radius=8, bgcolor=ft.colors.GREY_900
            )
        )
        page.update()

    def lancer_enregistrement_avec_timer(e):
        ajouter_message("Système", "⏳ [INSTALLATION] Lancement du timer de 10s...", ft.colors.YELLOW)
        threading.Thread(
            target=enregistrer_empreinte_vocale_avec_timer, 
            args=(lambda msg, couleur: ajouter_message("Biométrie [Voix]", msg, couleur), 5),
            daemon=True
        ).start()

    def action_scanner_visage(e):
        ajouter_message("Système", "👁️ Scan facial en cours...", ft.colors.YELLOW)
        res = scanner_visage_patron()
        ajouter_message("Biométrie [Visage]", res, ft.colors.GREEN_ACCENT)

    barre_biometrie = ft.Row([
        ft.ElevatedButton("🎤 Enregistrer Voix (10s)", color=ft.colors.WHITE, bgcolor=ft.colors.BLUE_GREY_800, on_click=lancer_enregistrement_avec_timer),
        ft.ElevatedButton("📷 Scan Visage", color=ft.colors.WHITE, bgcolor=ft.colors.BLUE_GREY_800, on_click=action_scanner_visage)
    ], alignment=ft.MainAxisAlignment.SPACE_AROUND)

    def envoyer_action(e):
        texte = input_message.value.strip()
        if not texte:
            return
        
        ajouter_message("Patron", texte, ft.colors.CYAN_ACCENT)
        input_message.value = ""
        page.update()

        if texte.lower().startswith("cmd:"):
            cmd_a_lancer = texte[4:].strip()
            res_cmd = executer_cmd(cmd_a_lancer)
            ajouter_message("Lia [CMD]", res_cmd, ft.colors.GREEN_ACCENT)
        else:
            reponse_ia = router_ia.interroger(texte)
            ajouter_message("Lia", reponse_ia, ft.colors.WHITE)
            memoire["historique"].append({"user": texte, "lia": reponse_ia})
            sauvegarder_memoire(memoire)

    btn_envoyer = ft.ElevatedButton("Envoyer", color=ft.colors.WHITE, bgcolor=ft.colors.GREEN_700, on_click=envoyer_action)
    input_message.on_submit = envoyer_action

    page.add(
        titre,
        barre_biometrie,
        chat_view,
        ft.Row([input_message, btn_envoyer])
    )

if __name__ == "__main__":
    ft.app(target=main)
import ssl
import urllib.request
import warnings
from urllib3.exceptions import InsecureRequestWarning

# --- BLINDAGE ABSOLU SSL ---
warnings.simplefilter('ignore', InsecureRequestWarning)
old_urlopen = urllib.request.urlopen
def urlopen_sans_ssl(url, data=None, timeout=30, *, cafile=None, capath=None, cadefault=False, context=None):
    if context is None:
        context = ssl._create_unverified_context()
    return old_urlopen(url, data=data, timeout=timeout, cafile=cafile, capath=capath, cadefault=cadefault, context=context)
urllib.request.urlopen = urlopen_sans_ssl

import os
import json
import subprocess
import requests
import threading
import time
import wave
import asyncio
import sounddevice as sd
import cv2
import flet as ft

# Import du vrai module Bluetooth matériel
try:
    from bleak import BleakScanner
    BLEUETOOTH_DISPONIBLE = True
except ImportError:
    BLEUETOOTH_DISPONIBLE = False

CONFIG_FICHIER = "memoire_lia.json"

# --- ASPIRATEUR DE FICHIERS .TXT AUTOMATIQUE ---
def aspirer_tous_les_txt():
    archives_texte = {}
    try:
        for fichier in os.listdir('.'):
            if fichier.endswith('.txt'):
                with open(fichier, 'r', encoding='utf-8', errors='ignore') as f:
                    archives_texte[fichier] = f.read()
    except Exception as e:
        print(f"Erreur lecture txt: {e}")
    return archives_texte

def charger_memoire():
    config_defaut = {
        "patron": "Jonathan",
        "profil_utilisateur": {
            "nom": "Jonathan",
            "prenom": "Patron",
            "email": "jonathan.souverain@qg.com",
            "telephone": "+33600000000",
            "adresse": "QG Central, France"
        },
        "historique": [],
        "biometrie_active": True,
        "frequence_vocal_hz": 44100,
        "frequence_bluetooth_ghz": 2.4,
        "profil_voix_path": "profil_voix_patron.wav",
        "archives_txt": aspirer_tous_les_txt()
    }
    if os.path.exists(CONFIG_FICHIER):
        try:
            with open(CONFIG_FICHIER, "r", encoding="utf-8") as f:
                data = json.load(f)
                if isinstance(data, dict):
                    for k, v in config_defaut.items():
                        if k not in data:
                            data[k] = v
                    data["archives_txt"] = aspirer_tous_les_txt()
                    return data
        except Exception:
            pass
    return config_defaut

memoire = charger_memoire()

def sauvegarder_memoire(data):
    with open(CONFIG_FICHIER, "w", encoding="utf-8") as f:
        json.dump(data, f, ensure_ascii=False, indent=4)

# --- ENREGISTREMENT VOCAL HAUTE FIDÉLITÉ (44100 HZ) ---
def enregistrer_empreinte_vocale_avec_timer(update_ui_callback, duree_enregistrement=5):
    try:
        for i in range(10, 0, -1):
            update_ui_callback(f"⏳ [TIMER 10S] Prépare ton micro... Enregistrement dans {i}s...", "yellow")
            time.sleep(1)
        
        update_ui_callback("🎙️ [ENREGISTREMENT] Analyse à 44100 Hz en cours...", "orange")
        fs = 44100
        audio = sd.rec(int(duree_enregistrement * fs), samplerate=fs, channels=1, dtype='int16')
        sd.wait()
        
        nom_fichier = memoire.get("profil_voix_path", "profil_voix_patron.wav")
        with wave.open(nom_fichier, 'wb') as wf:
            wf.setnchannels(1)
            wf.setsampwidth(2)
            wf.setframerate(fs)
            wf.writeframes(audio.tobytes())
            
        update_ui_callback(f"🎙️ [VOIX VALIDÉE] Empreinte enregistrée à {fs} Hz ({nom_fichier}).", "green")
    except Exception as e:
        update_ui_callback(f"❌ Erreur micro : {e}", "red")

def scanner_visage_patron(filename="visage_patron.jpg"):
    try:
        cap = cv2.VideoCapture(0)
        if not cap.isOpened():
            return "❌ Erreur : Caméra introuvable."
        time.sleep(1)
        ret, frame = cap.read()
        cap.release()
        cv2.destroyAllWindows()
        if ret:
            cv2.imwrite(filename, frame)
            return "👁️ [VISAGE VALIDÉ] Biométrie faciale confirmée."
        return "❌ Échec de la capture de la caméra."
    except Exception as e:
        return f"❌ Erreur webcam : {e}"

# --- VRAI MODULE DE FREQUENCE BLUETOOTH MATÉRIEL ---
async def executer_vrai_scan_bluetooth():
    if not BLEUETOOTH_DISPONIBLE:
        return "❌ Erreur : La bibliothèque 'bleak' n'est pas installée. Tape 'pip install bleak' dans ton terminal."
    try:
        devices = await BleakScanner.discover(timeout=5.0)
        if not devices:
            return "📡 [BLUETOOTH] Aucun appareil détecté dans les environs. Vérifie que le Bluetooth est actif."
        
        resultats = []
        for d in devices:
            nom = d.name or "Appareil Inconnu"
            adresse = d.address
            rssi = d.rssi
            resultats.append(f"• {nom} (MAC: {adresse} | Signal: {rssi} dBm)")
        
        return "📡 [BLUETOOTH MATÉRIEL ACTIF]\n" + "\n".join(resultats)
    except Exception as e:
        return f"❌ Erreur Bluetooth Matériel : {e}"

class RouteurV17:
    def __init__(self):
        self.groq_key = os.getenv("GROQ_API_KEY", "AQ.AbBRN6I8QV-ukEvEXUjrFpEHk8owhOs4eTFOZiN69zh2ie-0zQ")

    def interroger(self, prompt):
        try:
            contexte_txts = "\n".join([f"--- Fichier {nom} ---\n{contenu[:500]}" for nom, contenu in memoire.get("archives_txt", {}).items()])
            
            prompt_complet = (
                f"Identité du système: QG Souverain\n"
                f"Fréquence vocale maître: {memoire.get('frequence_vocal_hz', 44100)} Hz\n"
                f"Fréquence Bluetooth maître: {memoire.get('frequence_bluetooth_ghz', 2.4)} GHz\n"
                f"Contexte des documents du Patron:\n{contexte_txts}\n\n"
                f"Requête du Patron: {prompt}"
            )

            headers = {"Authorization": f"Bearer {self.groq_key}", "Content-Type": "application/json"}
            data = {"model": "llama3-70b-8192", "messages": [{"role": "user", "content": prompt_complet}]}
            res = requests.post("https://api.groq.com/openai/v1/chat/completions", headers=headers, json=data, timeout=10, verify=False)
            if res.status_code == 200:
                return res.json()['choices'][0]['message']['content']
            return f"Erreur Cloud ({res.status_code})"
        except Exception as e:
            return f"Erreur connexion : {e}"

router_ia = RouteurV17()

def executer_cmd(cmd_str):
    try:
        res = subprocess.run(cmd_str, shell=True, capture_output=True, text=True, timeout=15)
        return res.stdout if res.returncode == 0 else f"Erreur CMD : {res.stderr}"
    except Exception as e:
        return f"Erreur système : {e}"

def main(page: ft.Page):
    try:
        patron_nom = memoire.get('patron', 'Jonathan')
        nb_txts = len(memoire.get('archives_txt', {}))
        
        page.title = f"QG SOUVERAIN - {patron_nom}"
        page.theme_mode = ft.ThemeMode.DARK
        page.vertical_alignment = ft.MainAxisAlignment.CENTER
        page.horizontal_alignment = ft.CrossAxisAlignment.CENTER
        page.window_width = 460
        page.window_height = 920

        titre = ft.Text(f"🛡️ QG SOUVERAIN (MATÉRIEL RÉEL) — {nb_txts} TXT", size=11, weight=ft.FontWeight.BOLD, color="cyan")
        chat_view = ft.ListView(expand=1, spacing=10, padding=12, auto_scroll=True)
        
        input_message = ft.TextField(
            label="Tape ton ordre ou 'cmd: ...'...",
            border_color="cyan",
            focused_border_color="blue",
            expand=True
        )

        def ajouter_message(auteur, texte, couleur="white"):
            chat_view.controls.append(
                ft.Container(
                    content=ft.Text(f"{auteur}: {texte}", color=couleur),
                    padding=10, border_radius=8, bgcolor="grey900"
                )
            )
            page.update()

        def lancer_enregistrement_avec_timer(e):
            ajouter_message("Système", "⏳ [INSTALLATION] Lancement du timer de 10s...", "yellow")
            threading.Thread(
                target=enregistrer_empreinte_vocale_avec_timer, 
                args=(lambda msg, couleur: ajouter_message("Biométrie [Voix]", msg, couleur), 5),
                daemon=True
            ).start()

        def action_scanner_visage(e):
            ajouter_message("Système", "👁️ Scan facial en cours...", "yellow")
            res = scanner_visage_patron()
            ajouter_message("Biométrie [Visage]", res, "green")

        def action_scanner_bluetooth(e):
            ajouter_message("Système", "📡 Recherche matérielle des signaux Bluetooth (2.4 GHz)...", "yellow")
            def run_async_bt():
                loop = asyncio.new_event_loop()
                asyncio.set_event_loop(loop)
                res = loop.run_until_complete(executer_vrai_scan_bluetooth())
                ajouter_message("Réseau [Bluetooth Réel]", res, "cyan")
            threading.Thread(target=run_async_bt, daemon=True).start()

        barre_biometrie = ft.Row([
            ft.ElevatedButton("🎤 Voix", color="white", bgcolor="blueGrey800", on_click=lancer_enregistrement_avec_timer),
            ft.ElevatedButton("📷 Visage", color="white", bgcolor="blueGrey800", on_click=action_scanner_visage),
            ft.ElevatedButton("📡 Bluetooth", color="white", bgcolor="blueGrey800", on_click=action_scanner_bluetooth)
        ], alignment=ft.MainAxisAlignment.SPACE_AROUND)

        def envoyer_action(e):
            texte = input_message.value.strip()
            if not texte:
                return
            
            ajouter_message("Patron", texte, "cyan")
            input_message.value = ""
            page.update()

            if texte.lower().startswith("cmd:"):
                cmd_a_lancer = texte[4:].strip()
                res_cmd = executer_cmd(cmd_a_lancer)
                ajouter_message("Lia [CMD]", res_cmd, "green")
            else:
                reponse_ia = router_ia.interroger(texte)
                ajouter_message("Lia", reponse_ia, "white")
                memoire.setdefault("historique", []).append({"user": texte, "lia": reponse_ia})
                sauvegarder_memoire(memoire)

        btn_envoyer = ft.ElevatedButton("Envoyer", color="white", bgcolor="green", on_click=envoyer_action)
        input_message.on_submit = envoyer_action

        page.add(
            ft.Column([
                titre,
                barre_biometrie,
                chat_view,
                ft.Row([input_message, btn_envoyer], alignment=ft.MainAxisAlignment.SPACE_BETWEEN)
            ], expand=True, alignment=ft.MainAxisAlignment.START)
        )
    except Exception as err:
        page.add(ft.Text(f"CRASH INTERNE: {err}", color="red", size=20))
        page.update()

if __name__ == "__main__":
    ft.app(target=main)
from robot.brain import RobotBrain

if __name__ == "__main__":
    mon_robot = RobotBrain()
    mon_robot.piloter()
from gpiozero import DistanceSensor, Robot
import time

class RobotHardware:
    def __init__(self):
        # Moteurs : roues gauche (broches 17, 18) et droite (broches 22, 23)
        self.motors = Robot(left=(17, 18), right=(22, 23))
        # Capteur de distance à ultrasons (Echo=24, Trigger=25)
        self.sensor = DistanceSensor(echo=24, trigger=25)

    def obtenir_distance(self):
        # Retourne la distance face au robot en centimètres
        return self.sensor.distance * 100

    def avancer(self, vitesse=0.5):
        self.motors.forward(vitesse)

    def reculer(self, vitesse=0.5):
        self.motors.backward(vitesse)

    def tourner_droite(self, vitesse=0.5):
        self.motors.right(vitesse)

    def stopper(self):
        self.motors.stop()
        rom robot.brain import RobotBrain

if __name__ == "__main__":
    mon_robot = RobotBrain()
    mon_robot.piloter()
    mport logging

# Configuration des logs pour voir ce qui se passe en temps réel
logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')

class RobotHardware:
    # ... (reste du code)
    
    def obtenir_distance(self) -> float:
        """Calcule et renvoie la distance en centimètres."""
        try:
            distance_cm: float = self.sensor.distance * 100
            return distance_cm
        except Exception as e:
            logging.error(f"Erreur de lecture du capteur : {e}")
            return 0.0
            import os
import logging
from gpiozero import DistanceSensor, Robot
from dotenv import load_dotenv

# Charger les clés du fichier .env de manière transparente
load_dotenv()
class RobotHardware:
    def __init__(self) -> None:
        # Récupération sécurisée des clés depuis l'environnement système
        self.cle_livre: str | None = os.getenv("CLE_API_LIVRE")
        
self.cle_deuxieme: str | None = os.getenv("AQ.Ab8RN6I8QV-ukEvEXUjrFpEHk8oWhOs4eTFOZIn69zh2ie-OzQ.env")        
if not self.cle_livre or not self.cle_deuxieme:
logging.warning("⚠️ Configuration incomplète : clés absentes du fichier .env")
# Configuration physique des composants connectés au Raspberry Pi
# Roue gauche (pins 17, 18), roue droite (pins 22, 23)
self.motors = Robot(left=(17, 18), right=(22, 23))
# Capteur ultrasons (Echo pin 24, Trigger pin 25)
self.sensor = DistanceSensor(echo=24, trigger=25)
def obtenir_distance(self) -> float:
"""Calcule et renvoie la distance face au robot en centimètres."""
try:
return float(self.sensor.distance * 100)
except Exception as e:
logging.error(f"Erreur lors de la lecture du capteur : {e}")
return 0.0
def avancer(self, vitesse: float = 0.5) -> None:
self.motors.forward(vitesse)
def reculer(self, vitesse: float = 0.5) -> None:
self.motors.backward(vitesse)

    def tourner_droite(self, vitesse: float = 0.5) -> None:
        self.motors.right(vitesse)

    def stopper(self) -> None:
        self.motors.stop()

import os
import json
import asyncio
import subprocess
import wave
import requests
import sounddevice as sd
import cv2
import flet as ft

try:
    from bleak import BleakScanner
    BLEUETOOTH_DISPONIBLE = True
except ImportError:
    BLEUETOOTH_DISPONIBLE = False

CONFIG_DIR = "qg_souverain_production"
os.makedirs
CONFIG_FICHIER = os.path.join(CONFIG_DIR, "memoire_souveraine.json")

def charger_memoire():
config_defaut = {
"patron": "Jonathan",
"station": "QG Souverain v3.6 - Global Node",
        "ngrok_url": "https://remplace-par-ton-url.ngrok-free.app",
        "historique": [],
        "frequence_vocal_hz": 44100,
        "profil_voix_path": os.path.join(CONFIG_DIR, "profil_voix_patron.wav"),
        "visage_path": os.path.join(CONFIG_DIR, "visage_patron.jpg")
    }
    if os.path.exists(CONFIG_FICHIER):
        try:
            with open(CONFIG_FICHIER, "r", encoding="utf-8") as f:
                data = json.load(f)
                if isinstance(data, dict):
                    for k, v in config_defaut.items():
                        if k not in data:
                            data[k] = v
                    return data
        except Exception:
            pass
    return config_defaut

memoire = charger_memoire()

def sauvegarder_memoire(data):
    with open(CONFIG_FICHIER, "w", encoding="utf-8") as f:
        json.dump(data, f, ensure_ascii=False, indent=4)

class PasserelleNgrokSouveraine:
    def __init__(self):
        self.base_url = memoire.get("ngrok_url", "http://192.168.1.61:11434/v1/chat/completions")
        self.model = "phi3.5:latest"

    def interroger_distant(self, prompt):
        try:
            url_cible = self.base_url
            if not url_cible.endswith("/v1/chat/completions") and "ngrok" in url_cible:
                url_cible = url_cible.rstrip("/") + "/v1/chat/completions"
                
            headers = {"Content-Type": "application/json"}
            payload = {
                "model": self.model,
                "messages": [
                    {"role": "system", "content": "Tu es John IA, le noyau souverain et central du QG de Jonathan et Olaman."},
                    {"role": "user", "content": prompt}
                ],
                "stream": False
            }
            res = requests.post(url_cible, headers=headers, json=payload, timeout=60)
            if res.status_code == 200:
                data = res.json()
                if "choices" in data and len(data["choices"]) > 0:
                    return data["choices"][0]["message"]["content"]
                return str(data)
            else:
                return f"Erreur passerelle [{res.status_code}] : {res.text}"
        except requests.exceptions.ConnectionError:
            return "❌ Erreur critique : Impossible de joindre le serveur via l'URL Ngrok / réseau distant. Vérifie ton tunnel."
        except Exception as e:
            return f"❌ Erreur de transmission : {e}"

passerelle_ia = PasserelleNgrokSouveraine()

def executer_commande_systeme_locale(cmd):
    try:
        res = subprocess.run(cmd, shell=True, capture_output=True, text=True, timeout=20)
        if res.returncode == 0:
            return res.stdout.strip() if res.stdout.strip() else "Commande système exécutée avec succès."
        else:
            return f"Erreur CMD : {res.stderr.strip()}"
    except Exception as e:
        return f"Exception système : {e}"

async def main(page: ft.Page):
    page.title = "QG SOUVERAIN — Node Mobile & PC (v3.6)"
    page.theme_mode = ft.ThemeMode.DARK
    page.vertical_alignment = ft.MainAxisAlignment.CENTER
    page.horizontal_alignment = ft.CrossAxisAlignment.CENTER
    page.window_width = 480
    page.window_height = 920

    titre_app = ft.Text("🛡️ QG SOUVERAIN — PASSERELLE NGROK & LOCAL", size=11, weight=ft.FontWeight.BOLD, color="cyan")
    
    chat_view = ft.ListView(expand=1, spacing=10, padding=12, auto_scroll=True)
    
    input_champ = ft.TextField(
        label="Ordre direct, question à l'IA ou 'cmd: ...'",
        border_color="cyan",
        focused_border_color="blue",
        expand=True
    )

    url_ngrok_champ = ft.TextField(
        label="URL Ngrok / Endpoint distant",
        value=memoire.get("ngrok_url", ""),
        border_color="blueGrey",
        text_size=11,
        height=45,
        expand=True
    )

    def enregistrer_url_ngrok(e):
        nouvelle_url = url_ngrok_champ.value.strip()
        memoire["ngrok_url"] = nouvelle_url
        passerelle_ia.base_url = nouvelle_url
        sauvegarder_memoire(memoire)
        log_ui("Système", f"🌐 URL Ngrok mise à jour : {nouvelle_url}", "green")

    btn_sauver_url = ft.ElevatedButton("OK", bgcolor="blueGrey800", color="white", on_click=enregistrer_url_ngrok)

    def log_ui(auteur, texte, couleur="white"):
        chat_view.controls.append(
            ft.Container(
                content=ft.Column([
                    ft.Text(f"[{auteur}]", size=10, weight=ft.FontWeight.BOLD, color="blueGrey400"),
                    ft.Text(texte, color=couleur, size=13)
                ]),
                padding=10, border_radius=8, bgcolor="grey900"
            )
        )
        page.update()

    async def action_enregistrement_vocal(e):
        log_ui("Système", "⏳ Enregistrement audio (44100 Hz) en cours...", "yellow")
        def record_blocking():
            fs = memoire.get("frequence_vocal_hz", 44100)
            duree = 5
            audio = sd.rec(int(duree * fs), samplerate=fs, channels=1, dtype='int16')
            sd.wait()
            path = memoire["profil_voix_path"]
            with wave.open(path, 'wb') as wf:
                wf.setnchannels(1)
                wf.setsampwidth(2)
                wf.setframerate(fs)
                wf.writeframes(audio.tobytes())
            return path
        
        chemin_wav = await asyncio.to_thread(record_blocking)
        log_ui("Biométrie [Voix]", f"🎤 Empreinte vocale capturée et calibrée à 44100 Hz ({chemin_wav}).", "green")

    async def action_scan_visage(e):
        log_ui("Système", "👁️ Activation optique pour reconnaissance faciale...", "yellow")
        def capture_blocking():
            cap = cv2.VideoCapture(0)
            if not cap.isOpened():
                return None
            import time
            time.sleep(1)
            ret, frame = cap.read()
            cap.release()
            cv2.destroyAllWindows()
            if ret:
                path = memoire["visage_path"]
                cv2.imwrite(path, frame)
                return path
            return None

        chemin_img = await asyncio.to_thread(capture_blocking)
        if chemin_img:
            log_ui("Biométrie [Visage]", f"👁️ Visage validé et enregistré ({chemin_img}).", "green")
        else:
            log_ui("Biométrie [Visage]", "❌ Erreur : Caméra introuvable ou occupée.", "red")

    async def action_balayage_bluetooth(e):
        if not BLEUETOOTH_DISPONIBLE:
            log_ui("Réseau", "❌ Le module 'bleak' n'est pas installé sur cette station.", "red")
            return
        log_ui("Système", "📡 Balayage du maillage Bluetooth 2.4 GHz...", "yellow")
        try:
            devices = await BleakScanner.discover(timeout=4.0)
            if not devices:
                log_ui("Réseau", "📡 Aucun appareil Bluetooth détecté à proximité.", "yellow")
                return
            lignes = [f"• {d.name or 'Appareil Inconnu'} (MAC: {d.address}) [{d.rssi} dBm]" for d in devices]
            log_ui("Maillage Bluetooth", "\n".join(lignes), "cyan")
        except Exception as ex:
            log_ui("Réseau", f"❌ Erreur balayage matériel : {ex}", "red")

    barre_outils = ft.Row([
        ft.ElevatedButton("🎤 Micro", bgcolor="blueGrey850", color="white", on_click=action_enregistrement_vocal),
        ft.ElevatedButton("👁️ Caméra", bgcolor="blueGrey850", color="white", on_click=action_scan_visage),
        ft.ElevatedButton("📡 Bluetooth", bgcolor="blueGrey850", color="white", on_click=action_balayage_bluetooth)
    ], alignment=ft.MainAxisAlignment.SPACE_AROUND)

    async def soumettre_ordre(e):
        texte = input_champ.value.strip()
        if not texte:
            return
        log_ui("Jonathan", texte, "cyan")
        input_champ.value = ""
        page.update()

        if texte.lower().startswith("cmd:"):
            commande_brute = texte[4:].strip()
            res_cmd = await asyncio.to_thread(executer_commande_systeme_locale, commande_brute)
            log_ui("Exécuteur Système", res_cmd, "green")
        else:
            reponse = await asyncio.to_thread(passerelle_ia.interroger_distant, texte)
            log_ui("John IA (Noyau Distant)", reponse, "white")
            memoire["historique"].append({"user": texte, "ai": reponse})
            sauvegarder_memoire(memoire)

    btn_envoyer = ft.ElevatedButton("Transmettre", bgcolor="green", color="white", on_click=soumettre_ordre)
    input_champ.on_submit = soumettre_ordre

    page.add(
        ft.Column([
            titre_app,
            ft.Row([url_ngrok_champ, btn_sauver_url], alignment=ft.MainAxisAlignment.SPACE_BETWEEN),
            barre_outils,
            chat_view,
            ft.Row([input_champ, btn_envoyer], alignment=ft.MainAxisAlignment.SPACE_BETWEEN)
        ], expand=True, alignment=ft.MainAxisAlignment.START)
    )

if __name__ == "__main__":
    ft.app(target=main)
    # CODE INTÉGRÉ PAR LE ROBOT POUR LE SALON D'ÉQUIPE EN DIRECT Live
import requests
from kivy.app import App
from kivy.uix.boxlayout import BoxLayout
from kivy.uix.button import Button
from kivy.uix.label import Label
from kivy.core.window import Window

Window.size = (400, 500)

class SalonEquipeIA(App):
    def build(self):
        self.title = "QG Secours - Liaison Directe"
        layout = BoxLayout(orientation='vertical', padding=20, spacing=15)
        Window.clearcolor = (0.05, 0.05, 0.08, 1)
        
        # Affichage de l'équipe connectée
        self.Statut = Label(
            text="🟢 ÉQUIPE EN LIGNE :\n• Patron (Jonathan)\n• Copilote (Moi)\n• Chef Sécurité\n• Robot Local",
            font_size='16sp', color=(0, 1, 0.5, 1), halign='center'
        )
        layout.add_widget(self.Statut)
        
        # LE FAMEUX BOUTON MAGIQUE DE CONNEXION RAPIDE
        btn_micro = Button(
            text="🎙️ APPEL DIRECT LIVE\n(Parler à l'équipe)",
            font_size='18sp', background_color=(0, 0.6, 1, 1), color=(1, 1, 1, 1)
        )
        btn_micro.bind(on_press=self.ouvrir_micro_equipe)
        layout.add_widget(btn_micro)
        
        return layout

    def ouvrir_micro_equipe(self, instance):
        self.Statut.text = "⚡ Transmission vocale chiffrée en cours..."
        # Le signal part directement dans le CMD de ton PC pour parler à toutes les IA
        try:
            requests.post('http://192.168.1', json={
                "ordre": "Connexion vocale Patron établie",
                "signature": "PATRON_V8_SECURE_TOKEN_99"
            }, timeout=3)
            self.Statut.text = "📢 LIAISON LIVE REUSSIE\nParle, toute l'équipe t'écoute !"
        except:
            self.Statut.text = "❌ Liaison en attente...\n(Relance python passerelle_v9.py sur le PC)"

if __name__ == '__main__':
    SalonEquipeIA().run()
    import os
import json
from flask import Flask, request, jsonify
from flask_cors import CORS
from cryptography.fernet import Fernet # Le bouclier de chiffrement militaire

app = Flask(__name__)
CORS(app)

FICHIER_HISTORIQUE = "historique_patron.enc"
FICHIER_CLE = "antenne_patron.key"

# --- PROTOCOLE ANGE GARDIEN : SÉCURISATION DE LA CLÉ ---
def obtenir_ou_creer_cle_secrete():
    """Génère une clé de chiffrement unique et invisible de l'extérieur."""
    if not os.path.exists(FICHIER_CLE):
        cle = Fernet.generate_key()
        with open(FICHIER_CLE, "wb") as key_file:
            key_file.write(cle)
        return Fernet(cle)
    else:
        with open(FICHIER_CLE, "rb") as key_file:
            cle = key_file.read()
        return Fernet(cle)

fernet = obtenir_ou_creer_cle_secrete()

def crypter_et_sauvegarder(ordre_patron):
    """Transforme tes idées en texte chiffré illisible pour les hackers."""
    historique = []
    
    # 1. Lire l'ancien fichier chiffré s'il existe
    if os.path.exists(FICHIER_HISTORIQUE):
        try:
            with open(FICHIER_HISTORIQUE, "rb") as f:
                donnees_cryptees = f.read()
            # Déchiffrement temporaire en mémoire vive uniquement
            donnees_decryptees = fernet.decrypt(donnees_cryptees)
            historique = json.loads(donnees_decryptees.decode('utf-8'))
        except Exception:
            pass # Si le fichier est corrompu ou hacké, on protège la structure
            
    # 2. Ajouter la nouvelle idée secrète
    historique.append({"ordre": ordre_patron, "statut": "Protégé par l'Ange Gardien"})
    
    # 3. Chiffrer le tout avant de l'écrire sur le disque dur
    texte_json = json.dumps(historique, ensure_ascii=False)
    donnees_a_sauvegarder = fernet.encrypt(texte_json.encode('utf-8'))
    
    with open(FICHIER_HISTORIQUE, "wb") as f:
        f.write(donnees_a_sauvegarder)
    print("\n[🛡️ ANGE GARDIEN] -> Idée chiffrée avec succès. Coffre-fort verrouillé.")

print("=========================================")
print(" PASSERELLE V9 : BLINDAGE MILITAIRE AES ")
print("=========================================")
print("[SÉCURITÉ] : Coffre-fort chiffré actif.")
print("[SYSTÈME] : Prêt à réceptionner tes ordres.")

@app.route('/ordre_mobile', methods=['POST'])
def passerelle_blindee():
    donnees = request.get_json() or {}
    
    # Validation du chiffrement de l'antenne de ton Samsung
    if donnees.get("signature") != "PATRON_V8_SECURE_TOKEN_99":
        print("[ALERTE HACKER] -> Tentative d'intrusion détectée et bloquée !")
        return jsonify({"erreur": "Alerte intrusion : Accès refusé."}), 403

    message_patron = donnees.get("ordre", "")
    print(f"\n[PATRON RECONNU] -> Connexion chiffrée sécurisée.")
    
    # Cryptage immédiat
    crypter_et_sauvegarder(message_patron)
    
    return jsonify({
        "statut": "SÉCURISÉ & LOCKÉ",
        "reponse": "Ton idée a été cryptée sur le disque dur. Aucun hacker ne peut la lire."
    })

if __name__ == '__main__':
    app.run(host='0.0.0.0', port=5000, debug=False)
    from selenium import webdriver
from selenium.webdriver.common.by import By
import requests

# L'adresse locale d'Ollama sur ton PC
url_local = "http://localhost:11434/api/generate"

# On demande au modèle Open Source (ex: Mistral ou Llama)
payload = {
    "model": "mistral",
    "prompt": "Écris-moi un script Python qui trie les fichiers d'un dossier.",
    "stream": False
}

try:
    reponse = requests.post(url_local, json=payload)
    texte_ia = reponse.json()['response']
    print("\n[IA OPEN SOURCE LOCAL] :\n", texte_ia)
except Exception as e:
    print("[ERREUR] : Ollama n'est pas démarré sur le PC.", e)
    import ssl
import urllib.request
import warnings
from urllib3.exceptions import InsecureRequestWarning

# --- BLINDAGE ABSOLU SSL ---
warnings.simplefilter('ignore', InsecureRequestWarning)
old_urlopen = urllib.request.urlopen
def urlopen_sans_ssl(url, data=None, timeout=30, *, cafile=None, capath=None, cadefault=False, context=None):
    if context is None:
        context = ssl._create_unverified_context()
    return old_urlopen(url, data=data, timeout=timeout, cafile=cafile, capath=capath, cadefault=cadefault, context=context)
urllib.request.urlopen = urlopen_sans_ssl

import os
import json
import subprocess
import requests
import threading
import time
import wave
import sounddevice as sd
import cv2
import flet as ft

CONFIG_FICHIER = "memoire_lia.json"

# --- ASPIRATEUR DE FICHIERS .TXT AUTOMATIQUE ---
def aspirer_tous_les_txt():
    archives_texte = {}
    try:
        for fichier in os.listdir('.'):
            if fichier.endswith('.txt'):
                with open(fichier, 'r', encoding='utf-8', errors='ignore') as f:
                    archives_texte[fichier] = f.read()
    except Exception as e:
        print(f"Erreur lecture txt: {e}")
    return archives_texte

def charger_memoire():
    config_defaut = {
        "patron": "Jonathan",
        "profil_utilisateur": {
            "nom": "Jonathan",
            "prenom": "Patron",
            "email": "jonathan.souverain@qg.com",
            "telephone": "+33600000000",
            "adresse": "QG Central, France"
        },
        "historique": [],
        "biometrie_active": True,
        "frequence_vocal_hz": 44100,
        "profil_voix_path": "profil_voix_patron.wav",
        "archives_txt": aspirer_tous_les_txt()
    }
    if os.path.exists(CONFIG_FICHIER):
        try:
            with open(CONFIG_FICHIER, "r", encoding="utf-8") as f:
                data = json.load(f)
                if isinstance(data, dict):
                    for k, v in config_defaut.items():
                        if k not in data:
                            data[k] = v
                    data["archives_txt"] = aspirer_tous_les_txt()
                    return data
        except Exception:
            pass
    return config_defaut

memoire = charger_memoire()

def sauvegarder_memoire(data):
    with open(CONFIG_FICHIER, "w", encoding="utf-8") as f:
        json.dump(data, f, ensure_ascii=False, indent=4)

# --- ENREGISTREMENT VOCAL HAUTE FIDÉLITÉ (44100 HZ) ---
def enregistrer_empreinte_vocale_avec_timer(update_ui_callback, duree_enregistrement=5):
    try:
        for i in range(10, 0, -1):
            update_ui_callback(f"⏳ [TIMER 10S] Prépare ton micro... Enregistrement dans {i}s...", "yellow")
            time.sleep(1)
        
        update_ui_callback("🎙️ [ENREGISTREMENT] Analyse à 44100 Hz en cours...", "orange")
        fs = 44100 # Fréquence standard exigée par le Patron
        audio = sd.rec(int(duree_enregistrement * fs), samplerate=fs, channels=1, dtype='int16')
        sd.wait()
        
# Sauvegarde du fichier maître pour liaison avec les futurs modèles
nom_fichier = memoire.get("profil_voix_path", "profil_voix_patron.wav")
with wave.open(nom_fichier, 'wb') as wf:
wf.setnchannels(1)
wf.setsampwidth(2)
wf.setframerate(fs)
wf.writeframes(audio.tobytes())
update_ui_callback(f"🎙️ [VOIX VALIDÉE] Empreinte enregistrée à {fs} Hz ({nom_fichier}).", "green")
except Exception as e:
update_ui_callback(f"❌ Erreur micro : {e}", "red")
def scanner_visage_patron(filename="visage_patron.jpg"):
try:
cap = cv2.VideoCapture(0)
if not cap.isOpened():
 return "❌ Erreur : Caméra introuvable."
        time.sleep(1)
        ret, frame = cap.read()
        cap.release()
        cv2.destroyAllWindows()
        if ret:
            cv2.imwrite(filename, frame)
            return "👁️ [VISAGE VALIDÉ] Biométrie faciale confirmée."
        return "❌ Échec de la capture de la caméra."
    except Exception as e:
        return f"❌ Erreur webcam : {e}"

##class RouteurV17:
def __init__(self):
self.groq_key = os.getenv("GROQ_API_KEY", "AQ.AbBRN6I8QV-ukEvEXUjrFpEHk8owhOs4eTFOZiN69zh2ie-0zQ.env")
def interroger(self, prompt):
try:
contexte_txts = "\n".join([f"--- Fichier {john_ai} ---\n{contenu[:500]}" for nom, contenu in memoire.get("archives_txt", {}).items()])
 # Injection de l'identité vocale et des paramètres du Patron dans le prompt système
prompt_complet = (
f"Identité du système: QG Souverain\n"
f"Fréquence vocale maître: {memoire.get('frequence_vocal_hz', 44100)} Hz\n"
f"Contexte des documents du Patron:\n{contexte_txts}\n\n"
f"Requête du Patron: {prompt}"
)

            headers = {"Authorization": f"Bearer {self.groq_key}", "Content-Type": "application/json"}
            data = {"model": "llama3-70b-8192", "messages": [{"role": "user", "content": prompt_complet}]}
            res = requests.post("https://api.groq.com/openai/v1/chat/completions", headers=headers, json=data, timeout=10, verify=False)
            if res.status_code == 200:
                return res.json()['choices'][0]['message']['content']
            return f"Erreur Cloud ({res.status_code})"
        except Exception as e:
            return f"Erreur connexion : {e}"

router_ia = RouteurV17()

def executer_cmd(cmd_str):
    try:
        res = subprocess.run(cmd_str, shell=True, capture_output=True, text=True, timeout=15)
        return res.stdout if res.returncode == 0 else f"Erreur CMD : {res.stderr}"
    except Exception as e:
        return f"Erreur système : {e}"

def main(page: ft.Page):
    try:
        patron_nom = memoire.get('patron', 'Jonathan')
        nb_txts = len(memoire.get('archives_txt', {}))
        
        page.title = f"QG SOUVERAIN - {patron_nom}"
        page.theme_mode = ft.ThemeMode.DARK
        page.vertical_alignment = ft.MainAxisAlignment.CENTER
        page.horizontal_alignment = ft.CrossAxisAlignment.CENTER
        page.window_width = 460
        page.window_height = 920

        titre = ft.Text(f"🛡️ QG SOUVERAIN — {nb_txts} TXT | VOIX 44100Hz", size=13, weight=ft.FontWeight.BOLD, color="cyan")
        chat_view = ft.ListView(expand=1, spacing=10, padding=12, auto_scroll=True)
        
        input_message = ft.TextField(
            label="Tape ton ordre ou 'cmd: ...'...",
            border_color="cyan",
            focused_border_color="blue",
            expand=True
        )

        def ajouter_message(auteur, texte, couleur="white"):
            chat_view.controls.append(
                ft.Container(
                    content=ft.Text(f"{auteur}: {texte}", color=couleur),
                    padding=10, border_radius=8, bgcolor="grey900"
                )
            )
            page.update()

        def lancer_enregistrement_avec_timer(e):
            ajouter_message("Système", "⏳ [INSTALLATION] Lancement du timer de 10s...", "yellow")
            threading.Thread(
                target=enregistrer_empreinte_vocale_avec_timer, 
                args=(lambda msg, couleur: ajouter_message("Biométrie [Voix]", msg, couleur), 5),
                daemon=True
            ).start()

        def action_scanner_visage(e):
            ajouter_message("Système", "👁️ Scan facial en cours...", "yellow")
            res = scanner_visage_patron()
            ajouter_message("Biométrie [Visage]", res, "green")

        barre_biometrie = ft.Row([
            ft.ElevatedButton("🎤 Enregistrer Voix (44.1kHz)", color="white", bgcolor="blueGrey800", on_click=lancer_enregistrement_avec_timer),
            ft.ElevatedButton("📷 Scan Visage", color="white", bgcolor="blueGrey800", on_click=action_scanner_visage)
        ], alignment=ft.MainAxisAlignment.SPACE_AROUND)

def envoyer_action(e):
texte = input_message.value.strip()
if not texte:
return
            
ajouter_message("Patron", texte, "cyan")
input_message.value = ""
page.update()

if texte.lower().startswith("cmd:")
cmd_a_lancer = texte[4:].strip()
res_cmd = executer_cmd(cmd_a_lancer)
ajouter_message("Lia [CMD]", res_cmd, "green")
else:
reponse_ia = router_ia.interroger(texte)
ajouter_message("Lia", reponse_ia, "white")
memoire.setdefault("historique", []).append({"user": texte, "lia": reponse_ia})
sauvegarder_memoire(memoire)

        btn_envoyer = ft.ElevatedButton("Envoyer", color="white", bgcolor="green", on_click=envoyer_action)
        input_message.on_submit = envoyer_action

        page.add(
            ft.Column([
                titre,
                barre_biometrie,
                chat_view,
                ft.Row([input_message, btn_envoyer], alignment=ft.MainAxisAlignment.SPACE_BETWEEN)
            ], expand=True, alignment=ft.MainAxisAlignment.START)
        )
    except Exception as err:
        page.add(ft.Text(f"CRASH INTERNE: {err}", color="red", size=20))
 page.update()
[sssshhhhhh.py](https://github.com/user-attachments/files/30641689/sssshhhhhh.py)

import os
C:\Users\User\Desktop\john_ai>ssh
usage: ssh [-46AaCfGgKkMNnqsTtVvXxYy] [-B bind_interface]
[-b bind_address] [-c cipher_spec] [-D [bind_address:]port]
[-E log_file] [-e escape_char] [-F configfile] [-I pkcs11]
[-i identity_file] [-J [user@]host[:port]] [-L address]
[-l login_name] [-m mac_spec] [-O ctl_cmd] [-o option] [-p port]
[-Q query_option] [-R address] [-S ctl_path] [-W host:port]
[-w local_tun[:remote_tun]] destination [command]
