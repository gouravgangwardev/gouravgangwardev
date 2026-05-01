<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:060A07,25:0C1610,50:122318,75:1A3325,100:243D2F&height=280&section=header&text=GOURAV%20GANGWAR&fontSize=58&fontColor=B8CFAA&animation=fadeIn&fontAlignY=44&desc=Backend%20%E2%80%A2%20AI%20Systems%20%E2%80%A2%20Real-Time%20Infrastructure&descAlignY=62&descSize=16&fontAlign=50&descAlign=50" width="100%"/>

</div>

<br/>

<div align="center">

<a href="https://linkedin.com/in/gouravgangwardev"><img src="https://img.shields.io/badge/%E2%86%97%20LinkedIn-060A07?style=for-the-badge&logo=linkedin&logoColor=B8CFAA&labelColor=0C1610"/></a>&nbsp;
<a href="mailto:gouravgangwardev@gmail.com"><img src="https://img.shields.io/badge/%E2%86%97%20Email-060A07?style=for-the-badge&logo=gmail&logoColor=B8CFAA&labelColor=0C1610"/></a>&nbsp;
<a href="https://github.com/gouravgangwardev"><img src="https://img.shields.io/badge/%E2%86%97%20GitHub-060A07?style=for-the-badge&logo=github&logoColor=B8CFAA&labelColor=0C1610"/></a>

</div>

<br/>

<div align="center">

```
▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓
▓                                                              ▓
▓    Building systems where latency and scale collide.        ▓
▓    Distributed backends · AI inference · Real-time sync     ▓
▓                                                              ▓
▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓
```

</div>

<br/>

---

<br/>

## ❯ About

I'm a **Backend & Systems Engineer** who thrives under constraint — tight latency budgets, hostile failure modes, and scale that doesn't forgive sloppiness. My work sits at the seam between **distributed infrastructure**, **AI inference pipelines**, and **hardware-to-cloud systems**.

I don't just write code. I reason about systems — where they'll break, where they'll bottleneck, and how they should recover.

<br/>

---

<br/>

## ❯ Systems

<br/>

### ⬡ &nbsp;`BONDRA` &mdash; Real-Time Matchmaking Infrastructure

<table>
<tr>
<td width="50%">

**Problem**

Stateful matchmaking servers don't scale. Session stickiness kills horizontal growth. Load spikes during peak hours collapse naive architectures.

</td>
<td width="50%">

**Solution**

Redis sorted-set queues with O(log N) insertion. Pub/Sub decouples Socket.IO nodes — fully stateless, infinitely horizontal. Kubernetes handles burst scaling automatically.

</td>
</tr>
</table>

```
CLIENT ──► SOCKET.IO NODE (stateless) ──► REDIS PUB/SUB
                                               │
              ┌────────────────────────────────┘
              ▼
     SORTED-SET QUEUE  ──►  MATCHED PAIR EMIT  ──►  CLIENT
     O(log N) insert
```

| Metric | Implementation |
|--------|----------------|
| Queue complexity | `O(log N)` via Redis sorted sets |
| Session model | Stateless — all state externalized |
| Transport | Socket.IO over Pub/Sub |
| Scaling | Kubernetes HPA under sustained load |

<br/><br/>

---

### ⬡ &nbsp;`SCAM SENSE AI` &mdash; Fraud Detection System

<table>
<tr>
<td width="50%">

**Problem**

Fraudulent content is multi-modal — images with embedded text, PDFs with forged metadata, layered deception that defeats single-model approaches.

</td>
<td width="50%">

**Solution**

Layered detection: OCR extracts content, NLP classifies intent, dual ML models cross-validate. Ensemble consensus drives the final verdict.

</td>
</tr>
</table>

```
INPUT ──► OCR ENGINE ──► NLP CLASSIFIER ──┬──► MODEL A ──► ENSEMBLE
                                          └──► MODEL B ──► VERDICT (90%+ acc)
```

| Component | Approach | Performance |
|-----------|----------|-------------|
| Vision pipeline | OCR → feature extraction | Multi-modal |
| Classification | Dual ML ensemble | **90%+ accuracy** |
| Architecture | Layered defense | Fault-tolerant |

<br/><br/>

---

### ⬡ &nbsp;`SMART IOT MONITOR` &mdash; Edge-to-Cloud Sensor Pipeline

<table>
<tr>
<td width="50%">

**Problem**

Sensor data is continuous, noisy, high-frequency. Naive polling introduces latency. Unindexed time-series storage makes range queries unusable at scale.

</td>
<td width="50%">

**Solution**

ESP32 firmware pushes event-driven payloads. MongoDB time-series collections with compound indexes. Dashboard receives updates in under 500ms.

</td>
</tr>
</table>

```
ESP32 SENSOR ──► INGESTION API ──► MONGO TIME-SERIES INDEX
                                          │
                                          ▼
                               WEBSOCKET PUSH  ◄──── < 500ms
```

| Layer | Technology | SLA |
|-------|------------|-----|
| Edge device | ESP32 firmware | Hardware-level |
| Ingestion | REST / MQTT endpoint | Async |
| Storage | MongoDB time-series | Optimized range queries |
| Delivery | Event-driven push | **< 500ms** |

<br/><br/>

---

### ⬡ &nbsp;`NEURAL HOLOGRAPHY` &mdash; AI 3D Reconstruction System

<table>
<tr>
<td width="50%">

**Problem**

3D reconstruction from 2D input is compute-heavy and model-sensitive. Benchmarking across methods is essential — wrong architecture means unusable latency.

</td>
<td width="50%">

**Solution**

OpenCV preprocessing normalizes input. NeRF handles volumetric reconstruction. Gesture recognition provides natural interaction without hardware controllers.

</td>
</tr>
</table>

| Stage | Method |
|-------|--------|
| Capture & preprocess | OpenCV pipeline |
| 3D reconstruction | NeRF-based volumetric modeling |
| Benchmarking | Multi-model performance comparison |
| Interaction layer | Gesture recognition interface |

<br/>

---

<br/>

## ❯ Stack

<div align="center">

**Languages & Runtimes**

![Python](https://img.shields.io/badge/Python-060A07?style=for-the-badge&logo=python&logoColor=B8CFAA)
![TypeScript](https://img.shields.io/badge/TypeScript-0C1610?style=for-the-badge&logo=typescript&logoColor=B8CFAA)
![Node.js](https://img.shields.io/badge/Node.js-122318?style=for-the-badge&logo=node.js&logoColor=B8CFAA)
![C++](https://img.shields.io/badge/C++-1A3325?style=for-the-badge&logo=cplusplus&logoColor=B8CFAA)

**Data & Messaging**

![Redis](https://img.shields.io/badge/Redis-060A07?style=for-the-badge&logo=redis&logoColor=B8CFAA)
![MongoDB](https://img.shields.io/badge/MongoDB-0C1610?style=for-the-badge&logo=mongodb&logoColor=B8CFAA)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-122318?style=for-the-badge&logo=postgresql&logoColor=B8CFAA)
![Kafka](https://img.shields.io/badge/Kafka-1A3325?style=for-the-badge&logo=apachekafka&logoColor=B8CFAA)

**Infrastructure & Cloud**

![Docker](https://img.shields.io/badge/Docker-060A07?style=for-the-badge&logo=docker&logoColor=B8CFAA)
![Kubernetes](https://img.shields.io/badge/Kubernetes-0C1610?style=for-the-badge&logo=kubernetes&logoColor=B8CFAA)
![AWS](https://img.shields.io/badge/AWS-122318?style=for-the-badge&logo=amazon-aws&logoColor=B8CFAA)
![GCP](https://img.shields.io/badge/GCP-1A3325?style=for-the-badge&logo=google-cloud&logoColor=B8CFAA)

**AI / ML**

![PyTorch](https://img.shields.io/badge/PyTorch-060A07?style=for-the-badge&logo=pytorch&logoColor=B8CFAA)
![OpenCV](https://img.shields.io/badge/OpenCV-0C1610?style=for-the-badge&logo=opencv&logoColor=B8CFAA)
![scikit-learn](https://img.shields.io/badge/scikit--learn-122318?style=for-the-badge&logo=scikit-learn&logoColor=B8CFAA)

</div>

<br/>

---

<br/>

## ❯ Focus Areas

<br/>

```
┌───────────────────────────┬──────────────────────────────────────────────────┐
│  DISTRIBUTED SYSTEMS      │  Consensus, partitioning, fault tolerance,        │
│                           │  CAP tradeoffs, eventual consistency              │
├───────────────────────────┼──────────────────────────────────────────────────┤
│  REAL-TIME SYNC           │  Sub-second pipelines, WebSocket architecture,    │
│                           │  pub/sub patterns, event-driven design            │
├───────────────────────────┼──────────────────────────────────────────────────┤
│  AI INFERENCE             │  Model serving, multi-modal pipelines,            │
│                           │  latency-aware deployment, ensemble methods       │
├───────────────────────────┼──────────────────────────────────────────────────┤
│  PERFORMANCE ENGINEERING  │  Profiling, benchmarking, algorithmic complexity, │
│                           │  load modeling, capacity planning                 │
└───────────────────────────┴──────────────────────────────────────────────────┘
```

<br/>

---

<br/>

## ❯ GitHub Activity

<br/>

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=gouravgangwardev&show_icons=true&theme=transparent&hide_border=true&title_color=B8CFAA&text_color=7A9E72&icon_color=4A7C59&bg_color=060A07&border_radius=6" height="165"/>
&nbsp;&nbsp;
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=gouravgangwardev&layout=compact&theme=transparent&hide_border=true&title_color=B8CFAA&text_color=7A9E72&bg_color=060A07&border_radius=6&langs_count=6" height="165"/>

</div>

<div align="center">

<img src="https://github-readme-streak-stats.herokuapp.com?user=gouravgangwardev&theme=transparent&hide_border=true&stroke=1A3325&ring=4A7C59&fire=B8CFAA&currStreakLabel=B8CFAA&sideLabels=7A9E72&dates=4A6A52&currStreakNum=B8CFAA&sideNums=B8CFAA&background=060A07" height="165"/>

</div>

<br/>

---

<br/>

## ❯ Principles

<br/>

<div align="center">

> **Latency is not a feature. It is a constraint. Design for it first.**

> **Reliability is not a property of components. It is a property of systems.**

> **Execution over everything.**

</div>

<br/>

---

<br/>

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:243D2F,35:1A3325,65:0C1610,100:060A07&height=140&section=footer&text=flow%20%C2%B7%20depth%20%C2%B7%20systems&fontSize=13&fontColor=3D6B4F&fontAlignY=70" width="100%"/>

</div>
