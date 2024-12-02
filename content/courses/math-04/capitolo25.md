---
title: I Numeri Complessi
linktitle: Capitolo 25 Trigonometria
toc: true
type: docs
date: "2019-05-05T00:00:00+01:00"
draft: false
menu:
  math-04:
    parent:
    weight: 50

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 20
---

> ☆ **scadenza**: 30 ottobre 2021

![ex2_img](../ex2_img.png)

# Trigonometria

> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat.

Proin tincidunt magna sed ex sollicitudin condimentum. Sed ac faucibus dolor, scelerisque sollicitudin nisi. Cras purus urna, suscipit quis sapien eu, pulvinar tempor diam.

## Introduzione ai Numeri Complessi

## Obiettivi della lezione

- Comprendere la necessità di ampliare il concetto di numero per risolvere equazioni come $x^2 + 1 = 0$.
- Introdurre la definizione di numero complesso.
- Esplorare le rappresentazioni algebrica e geometrica dei numeri complessi.
- Presentare applicazioni reali e interdisciplinari.

---

## Perché servono i numeri complessi?

### Un problema storico

- Immaginiamo di voler risolvere questa equazione:
  $$x^2 + 1 = 0$$
  - Le radici sarebbero $x = \pm \sqrt{-1}$, ma non possiamo calcolare la radice quadrata di un numero negativo nei numeri reali.
  - Questo problema portò i matematici a introdurre una nuova "entità": $i$, dove:
    $$i^2 = -1$$

### Un esempio accattivante: l'elettricità alternata

- **Domanda intrigante per la classe**: Come funzionano le reti elettriche che portano energia a casa nostra?
- Risposta: Le oscillazioni della corrente alternata sono descritte usando numeri complessi:
  $$V(t) = V_0 e^{i\omega t}$$
  dove $i$ aiuta a modellare la fase e l'ampiezza in modo elegante.

---

## Definizione di numero complesso

- Un numero complesso è della forma:
  $$z = a + bi$$
  dove:
  - $a$ è la **parte reale** ($\Re(z)$).
  - $b$ è la **parte immaginaria** ($\Im(z)$).
  - $i$ è l'unità immaginaria, con $i^2 = -1$.

---

### Le 3 forme di un numero complesso

#### Forma algebrica

La forma algebrica di un numero complesso è:

$$
z=a+b i
$$

dove:

- $a \in \mathbb{R}$ è la parte reale,
- $b \in \mathbb{R}$ è la parte immaginaria,
- $i$ è l'unità immaginaria, tale che $i^2=-1$.

2. Forma trigonometrica

#### La forma trigonometrica è

$$
z=r(\cos \theta+i \sin \theta)
$$

dove:

- $r=|z|=\sqrt{a^2+b^2}$ è il modulo di $z$,
- $\theta=\arg (z)$ è l'argomento (o fase) di $z$, con $\theta \in[0,2 \pi)$,
- $\cos \theta$ e $\sin \theta$ sono le proiezioni di $z$ sull'asse reale e immaginario.

3. Forma esponenziale

#### La forma esponenziale

- derivata dalla forma trigonometrica usando la formula di Eulero $e^{i \theta}=$ $\cos \theta+i \sin \theta$, è:

$$
z=r e^{i \theta}
$$

dove:

- $r=|z|$ è il modulo,
- $\theta=\arg (z)$ è l'argomento.

#### Relazioni tra le forme

Dato un numero complesso $z=a+b i$ :

- Il modulo è:

$$
r=|z|=\sqrt{a^2+b^2}
$$

- L'argomento è:

$$
\left.\theta=\arctan \left(\frac{b}{a}\right) \quad \text { (con attenzione al quadrante del punto }(a, b)\right) .
$$

- La forma trigonometrica si converte facilmente in quella esponenziale con:

$$
\cos \theta+i \sin \theta=e^{i \theta}
$$

## Rappresentazione geometrica

- I numeri complessi possono essere rappresentati sul **piano di Gauss**, con:
  - L'asse $x$ come parte reale.
  - L'asse $y$ come parte immaginaria.
- Esempio:
  - $z = 3 + 4i$ corrisponde al punto $(3, 4)$.

### Modulo e argomento

- Il **modulo** di $z = a + bi$:
  $$|z| = \sqrt{a^2 + b^2}$$
- L'**argomento** (angolo con l'asse reale):
  $$\theta = \arctan\left(\frac{b}{a}\right)$$

---

## Applicazioni e interdisciplinarità

1. **Elettronica e ingegneria**:
   - Simulazione di circuiti con numeri complessi per modellare corrente e tensione.
2. **Grafica computerizzata**:
   - I frattali, come il famoso [[20 MATHS/21 Math's Drafts Inbox/insieme di Mandelbrot]], sono costruiti iterando funzioni di numeri complessi.
3. **Fisica quantistica**:
   - Le funzioni d'onda descrivono stati quantistici usando numeri complessi.

---

## Esercizio finale: un esempio pratico

### Problema

- Calcolare il modulo e l'argomento del numero complesso:
  $$z = -3 + 4i$$

### Soluzione

- Modulo:
  $$|z| = \sqrt{(-3)^2 + 4^2} = 5$$
- Argomento:
  $$\theta = \arctan\left(\frac{4}{-3}\right) \approx 126.87^\circ$$

---

## L'identità di Eulero: $e^{i\pi} + 1 = 0$

### Perché è considerata "la formula più bella"?

- L'**identità di Eulero** collega tra loro cinque delle costanti più importanti della matematica:
  - **$e$**: la base dei logaritmi naturali, fondamentale nell'analisi matematica e nei fenomeni di crescita esponenziale.
  - **$i$**: l'unità immaginaria, che permette di ampliare il concetto di numero.
  - **$\pi$**: la costante che esprime il rapporto tra la circonferenza e il diametro di un cerchio, onnipresente in geometria e trigonometria.
  - **$1$**: l'identità moltiplicativa, essenziale in tutte le strutture algebriche.
  - **$0$**: l'elemento neutro dell'addizione, simbolo del nulla e punto di origine in molte rappresentazioni.
- È sorprendente come queste costanti, apparentemente scollegate, si uniscano in una relazione così semplice e compatta.

---

### Le basi teoriche: la formula di Eulero

- L'identità di Eulero deriva dalla formula di Eulero, che esprime il legame tra esponenziali complessi e funzioni trigonometriche:
  $$e^{i\theta} = \cos(\theta) + i\sin(\theta)$$
- Questa formula si basa sull'espansione in serie di Taylor delle funzioni esponenziale, seno e coseno:
  $$e^x = 1 + \frac{x}{1!} + \frac{x^2}{2!} + \frac{x^3}{3!} + \dots$$
  $$\cos(x) = 1 - \frac{x^2}{2!} + \frac{x^4}{4!} - \dots$$
  $$\sin(x) = x - \frac{x^3}{3!} + \frac{x^5}{5!} - \dots$$
- Sostituendo $x = i\theta$, i termini si combinano in modo tale da collegare esponenziali e trigonometria.

![[50 Allegati/Pasted image 20241128222307.png]]

---

### Dimostrazione dell'identità di Eulero

1. Applicando la formula di Eulero per $\theta = \pi$:
   $$e^{i\pi} = \cos(\pi) + i\sin(\pi)$$
2. Valutando i termini trigonometrici:
   - $\cos(\pi) = -1$, perché il punto corrispondente a $\pi$ sulla circonferenza unitaria si trova a sinistra dell'origine.
   - $\sin(\pi) = 0$, perché il punto è sull'asse reale.
3. Quindi:
   $$e^{i\pi} = -1$$
4. Aggiungendo $1$ a entrambi i membri:
   $$e^{i\pi} + 1 = 0$$

---

### Interpretazione geometrica

- La formula $e^{i\theta} = \cos(\theta) + i\sin(\theta)$ rappresenta un punto sulla circonferenza unitaria nel piano complesso.
- Per $\theta = \pi$, il punto si trova all'estremità opposta rispetto all'origine, corrispondente a $-1$.
- L'identità $e^{i\pi} + 1 = 0$ può essere vista come una "chiusura del cerchio": l'esponenziale complesso con $\pi$ come angolo porta esattamente a $-1$.

---

### Applicazioni e significato

- **Analisi matematica**: $e^{i\pi}$ combina crescita esponenziale e oscillazioni sinusoidali.
- **Fisica**: appare in fenomeni ondulatori, quantistici e nella descrizione delle rotazioni.
- **Ingegneria**: è alla base della trasformata di Fourier, usata in elaborazione dei segnali.
- **Filosofia matematica**: rappresenta l'armonia e l'eleganza della matematica, collegando concetti apparentemente distanti in un'unica relazione.
