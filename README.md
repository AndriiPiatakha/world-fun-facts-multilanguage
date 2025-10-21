# 🌍 Global Fun Facts Multilanguage FREE API

The **Global Fun Facts API** is the most complete and verified database of fun, educational, and cultural facts in the world — available in **100+ languages** and growing every week.

<p align="center">
  🆓 <b>FREE API</b> — use instantly on 
  <a href="https://rapidapi.com/vintarok-vintarok-default/api/world-fun-facts-all-languages-support" target="_blank"><b>RapidAPI</b></a> 🚀
</p>

<p align="center">
  <a href="https://rapidapi.com/vintarok-vintarok-default/api/world-fun-facts-all-languages-support">
    <img src="logo.png" width="120" alt="Fun Facts API Logo">
  </a>
</p>

Instantly fetch random or specific facts by UUID, perfectly localized for your users. Whether you’re building a trivia app, a global learning platform, a travel project, or a multilingual chatbot — this API gives you engaging, localized facts from every corner of the world.

---

## 💎 Why It’s Unique

- 🗂 **The largest verified fun-facts collection online**  
- 🌐 **100+ supported languages**, including English, Russian, Spanish, French, German, Italian, Portuguese, Chinese (Mandarin), Japanese, Polish, Arabic, Hindi, Turkish, Dutch, Korean, Vietnamese, Indonesian, Thai, Persian, Ukrainian, Romanian, Czech, Greek, Hebrew, Swedish, Danish, Finnish, Norwegian, Hungarian, Serbian, Croatian, Bulgarian, Slovak, Slovenian, Lithuanian, Latvian, Estonian, Georgian, Armenian, Azerbaijani, Kazakh, Uzbek, Tamil, Telugu, Malayalam, Marathi, Punjabi, Gujarati, Sinhala, Swahili, Afrikaans, Amharic, Nepali, Burmese, Khmer, Mongolian, and Latin.  
- 🌏 Perfect for **internationalization (i18n)**, **education**, **entertainment**, **language learning**, **media**, and **social bots**.  
- ⚡ **Simple, fast, and secure JSON REST endpoint** with human-quality localized texts.

---

## 💡 Need a New Language?
If your language isn’t on the list — just contact us through the RapidAPI support section. We’ll add a new one **within a few days**.

---

## 🎯 Use Cases

- 🌍 **Multilingual mobile apps and websites**  
- 🎮 **Trivia games and daily “Did You Know?” features**  
- 📚 **Educational and e-learning platforms**  
- 💬 **Language learning content and chatbots**  
- 📰 **Media, newsletters, and global social channels**  

---

## ✨ Highlights

- 🎲 **Random or UUID-based fact retrieval**  
- 🈳 **Automatic localization for 100+ languages**  
- ✅ **Verified, unique, and curated database**  
- 🌎 **Designed for international reach and cross-cultural engagement**  

---

## 🔑 Keywords

fun facts, trivia, global facts, world facts, multilingual api, translation api, education, entertainment, random facts api, verified data, internationalization, i18n, cultural content, learning, knowledge, daily facts, language learning, world culture, language api, facts generator, global trivia, multilingual content, world knowledge, localization api, global entertainment


# 🌍 Global Fun Facts API

Discover **verified fun facts from around the world** — localized into **100+ languages** and ready for your multilingual app, website, or educational project.  
With this API, you can fetch random or specific facts (via UUID), automatically translated and stored for reuse.

---

## 🚀 Overview

The **Global Fun Facts API** provides access to one of the world’s most complete collections of educational, entertaining, and cultural fun facts — each fact available in more than 60 languages.

**Key Highlights:**
- 🌐 100+ supported languages  
- 🧩 Random or UUID-based fact retrieval  
- 💬 Automatic localization and caching  
- 🔒 Secure and production-ready JSON REST API  
- 📚 Perfect for trivia, learning apps, chatbots, or global content feeds  

If your language isn’t supported yet — contact us.  
We’ll add it **within a few days** 📧  


---

## 🧭 Endpoint: `GET /fact.php`

### Description
Fetches a **random fun fact** or a **specific fact by UUID** in the requested language.  
If the fact is not yet translated, the API automatically translates and stores it.

---

### 🔍 Query Parameters

| Name | Type | Required | Description | Example |
|------|------|-----------|--------------|----------|
| `lang` | `string` | ❌ Optional | Two-letter ISO language code (or full name). Default is 'en'. | `fr`, `es`, `ru` |
| `uuid` | `string` | ❌ Optional | UUID of a specific fact. If not provided, returns a random fact. | `df6dae1dba517a24b85a3dccca293eaa` |

---

### 🌎 Supported Languages

| Code | Language Name | Code | Language Name |
|------|----------------|------|----------------|
| en | English | ru | Russian |
| es | Spanish | fr | French |
| de | German | it | Italian |
| pt | Portuguese | zh | Chinese (Mandarin) |
| ja | Japanese | pl | Polish |
| ar | Arabic | hi | Hindi |
| bn | Bengali | ur | Urdu |
| tr | Turkish | nl | Dutch |
| ko | Korean | vi | Vietnamese |
| id | Indonesian | th | Thai |
| fa | Persian | ua | Ukrainian |
| ro | Romanian | cs | Czech |
| el | Greek | he | Hebrew |
| sv | Swedish | da | Danish |
| fi | Finnish | no | Norwegian |
| hu | Hungarian | sr | Serbian |
| hr | Croatian | bg | Bulgarian |
| sk | Slovak | sl | Slovenian |
| lt | Lithuanian | lv | Latvian |
| et | Estonian | ka | Georgian |
| hy | Armenian | az | Azerbaijani |
| kk | Kazakh | uz | Uzbek |
| tk | Turkmen | ta | Tamil |
| te | Telugu | ml | Malayalam |
| mr | Marathi | pa | Punjabi |
| gu | Gujarati | si | Sinhala |
| sw | Swahili | af | Afrikaans |
| am | Amharic | ne | Nepali |
| my | Burmese | km | Khmer |
| mn | Mongolian | la | Latin |

---

## 💬 Example Requests

### 🔸 Random Fact (Default English)
```bash
curl "/fact.php?lang=en"
```

### 🔸 French Version
```bash
curl "/fact.php?lang=fr"
```

### 🔸 Specific Fact by UUID (in Spanish)
```bash
curl "/fact.php?lang=es&uuid=df6dae1dba517a24b85a3dccca293eaa"
```

---

## 💡 Example Responses

### ✅ Success
```json
{
  "ok": true,
  "uuid": "df6dae1dba517a24b85a3dccca293eaa",
  "lang_code": "fr",
  "lang_name": "French",
  "text": "Le 10 janvier est la Journée des gens bizarres — pour célébrer ceux d'entre nous qui sont un peu excentriques."
}
```

### ⚠️ Error (Unsupported Language)
```json
{
  "ok": false,
  "error": "Unsupported language",
  "supported_codes": ["en", "ru", "es", "fr", "..."]
}
```

---

## 📚 Use Cases

- 🧠 **Educational apps:** Daily trivia or language-learning content  
- 🌎 **Global media & blogs:** Multilingual “Did you know?” sections  
- 🤖 **Chatbots:** Fun facts in users’ native languages  
- 🎡 **Games:** Random trivia for international audiences  
- 📱 **Localization:** Global content feeds and cross-cultural education tools  


---

## ⚠️ Terms of Use

The **Free plan** is strictly for **non-commercial, personal, and educational use only** — ideal for learning, fun, and testing.  
Commercial, automated, or redistributed usage requires a **paid plan**.  
Abuse or excessive automated traffic may result in suspension.

---

## 🥩 Developer Notes

- If translation for a fact doesn’t exist, it’s generated instantly and stored.  
- Facts are globally unique, referenced by `uuid`.  
- Each translation is permanently cached for performance.  
- Fast MySQL backend with optimized query logic.

---

## 🏷️ Keywords

fun facts, trivia, global facts, multilingual api, random facts, education, entertainment, culture, localization, i18n, world knowledge, learning api, daily facts, translation api, internationalization, multilingual content

---

## 📩 Support

For technical issues or new language requests:  
Contact Vintarok Team via RapidAPI messages.
We typically respond within **24–48 hours**.

---


