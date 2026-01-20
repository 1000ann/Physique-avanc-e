# Physique avancée
L'objectif premier est de transmettre des valeurs de température d'un LM35 à une Raspberry Pi via MQCC. 

# 🌡️ Système de Surveillance de Température – ESP32, MQTT & Raspberry Pi

## 📌 Présentation du projet

Ce projet consiste à concevoir un **système de surveillance de température** basé sur un **ESP32**, un **capteur LM35**, un **Raspberry Pi** et le protocole **MQTT**.  
Les données de température sont transmises par l’ESP32 vers un broker MQTT (Mosquitto), stockées dans une **base de données SQLite** sur le Raspberry Pi, puis affichées en temps réel via **Node-RED**.

Le système intègre également :
- une **gestion basse consommation** côté ESP32,
- une **sécurisation des communications MQTT**,
- des **alertes automatiques** en cas de dépassement de seuil,
- et une **documentation complète**.

---

## 🧱 Architecture générale

LM35 → ESP32 → MQTT (Mosquitto) → Raspberry Pi
↓
SQLite
↓
Node-RED
↓
Dashboard & Alertes

---

## 🎯 Objectifs du projet

- Mesurer la température ambiante avec un capteur LM35
- Transmettre les données via MQTT
- Réduire la consommation électrique de l’ESP32
- Stocker les mesures dans une base SQLite
- Visualiser les données en temps réel
- Déclencher des alertes si un seuil est dépassé
- Sécuriser les communications MQTT

---

## 🛠️ Matériel et logiciels utilisés

### Matériel
- ESP32
- Capteur de température LM35
- Raspberry Pi
- LED (ou LED RGB)
- Câbles de connexion

### Logiciels
- Arduino IDE
- Mosquitto (broker MQTT)
- SQLite
- Node-RED
- Python
- Git / GitHub

---

## 🚀 Mise en route – Premières étapes

### 1️⃣ Préparation du Raspberry Pi

Mettre à jour le système :
```bash
sudo apt update
sudo apt upgrade
