# 📊 Pushshift Reddit Dataset Analysis

Welcome! This repository explores the **Pushshift Reddit Dataset**, one of the most comprehensive, large-scale datasets available for analyzing online discourse, community behavior, and social trends on Reddit.

> “The front page of the Internet” — now available in billions of comments and posts.

---

## 🔍 Overview

The **Pushshift Reddit Dataset** contains:
- 📅 Data from **June 2005 to present**
- 🗃️ **651M+ submissions** and **5.6B+ comments**
- 💬 Data spanning **2.8M+ subreddits**

This project leverages the dataset to study topics such as:
- Online extremism and disinformation
- Community moderation and governance
- Mental health, radicalization, and harassment patterns
- Engagement and virality dynamics
- Sentiment, toxicity, and lexical patterns over time

---

## 📁 Dataset Access

| Resource | Description |
|----------|-------------|
| [Pushshift API](https://pushshift.io/api-parameters/) | Search and filter Reddit data on-the-fly |
| [Monthly Dumps](https://files.pushshift.io/reddit/) | Full datasets (comments & submissions by month) |
| [Zenodo Sample](https://doi.org/10.5281/zenodo.3608135) | Citable dataset DOI (sample only) |

---

## 🧠 Use Cases

Here are some domains where this dataset shines:

### 1. **Computational Social Science**
- Topic modeling
- Norms & behavior evolution
- Community formation & collapse

### 2. **Extremism & Disinformation Studies**
- Track hate speech, propaganda, radicalization
- Study spillover from fringe to mainstream platforms

### 3. **NLP & Machine Learning**
- Sentiment analysis, sarcasm detection, summarization
- Bot detection and fake account modeling

### 4. **Health Informatics**
- Depression, addiction, and disorder detection from posts
- Temporal tracking of public health discussions

---

## 🛠 Technologies Used

- 📦 `ndjson` formatted files for efficient processing
- 🔍 `ElasticSearch` & `PostgreSQL` for search and storage
- 🚀 Real-time data collection with a robust **Ingest Engine**
- 📊 API + Slackbot for interactive querying and visualization

---

## 🔧 Data Structure

### Submissions (per line in `.ndjson`)
| Field | Description |
|-------|-------------|
| `title`, `selftext` | Post content |
| `author`, `subreddit` | Metadata |
| `score`, `num_comments` | Engagement metrics |
| `created_utc` | UNIX timestamp |

### Comments (per line in `.ndjson`)
| Field | Description |
|-------|-------------|
| `body` | Comment text |
| `link_id`, `parent_id` | Thread info |
| `score`, `gilded`, `controversiality` | Community reaction |
| `created_utc` | UNIX timestamp |

---

## 📈 Example Analyses (Ideas to Implement)

- 🧵 Topic modeling with LDA on comments during 2020 elections  
- 🚫 Hate speech trend analysis across banned subreddits  
- 🧠 Mental health keyword detection over time in /r/depression  
- 🔗 Network graph of subreddit co-commenting behavior

---

## 🧑‍🤝‍🧑 Community & Collaboration

- [r/pushshift](https://www.reddit.com/r/pushshift): Community updates
- Slackbot: Real-time queries, visualization support
- Used in 100+ peer-reviewed papers across CS, sociology, health, and media

---

## 🧾 Citation

If you use this dataset, cite:

> Baumgartner et al. “The Pushshift Reddit Dataset.”  
> *Proceedings of ICWSM 2020*.  
> DOI: [10.5281/zenodo.3608135](https://doi.org/10.5281/zenodo.3608135)

---

## ⚖️ License & FAIR Principles

Pushshift data follows FAIR principles:
- **Findable**: Indexed monthly dumps + DOI
- **Accessible**: Publicly downloadable + API
- **Interoperable**: Standard JSON/ndjson formats
- **Reusable**: Clear provenance, research-friendly

---

## 📬 Contact

For academic collaboration or questions:
- [Pushshift.io](https://pushshift.io)
- [Jason Baumgartner](mailto:jason@pushshift.io)

---

> If you’re exploring Reddit at scale — this is your launchpad.
