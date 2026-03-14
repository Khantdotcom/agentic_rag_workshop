# 📋 Pre-Session Slides: Agentic RAG Workshop

## Translated English textbefore class (15-20 Translated English text workshop)

---

## Slide 1: Translated English text
- **Agentic RAG: From Zero to Hero**
- Workshop 4 Translated English text
- Translated English text ICT Translated English text

---

## Slide 2: learning outcomes
- ✂️ Translated English text RAG (Chunk → Embed → VectorDB)
- 🤖 Translated English text AI Agent Translated English text Google ADK
- ⭐ Translated English text **Agentic RAG** — Agent Translated English text + Translated English text + Translated English text
- 📊 Translated English text LLM-as-Judge

---

## Slide 3: Timeline Translated English text Workshop
| Part     |     Translated English text     | content                                  |
| -------- | :----------: | -------------------------------------- |
| 📢 Part 1 | 1 Translated English text. 20 Translated English text | Data Pipeline: Chunk → Embed → Qdrant  |
| ☕ Translated English text     |    10 Translated English text    |                                        |
| 📢 Part 2 | 1 Translated English text. 30 Translated English text | Agent → Tool → RAG Agent → Agentic RAG |
| 🧪 Part 3 |    1 Translated English text.     | Translated English text (10 points) + Q&A               |

---

## Slide 4: 🌐 Translated English text — myhero.megawiz.co.th

### Translated English text
1. Translated English text **[myhero.megawiz.co.th/student-portal](https://myhero.megawiz.co.th/student-portal/)**
2. Translated English text **Translated English text** Translated English text OTP
3. Translated English text OTP Translated English text → Translated English text
4. Translated English text **Translated English text-Translated English text** Translated English text **Translated English textstudents**

### Translated English text
- 📄 Translated English text (Notebook)
- 📝 Translated English text + Translated English text
- 🏆 **Certificate** Translated English text workshop

> 🎯 **Translated English text** Translated English text workshop Translated English text

---

## Slide 5: ⚠️ Translated English text

1. ✅ **Translated English text** Translated English text [myhero.megawiz.co.th/student-portal](https://myhero.megawiz.co.th/student-portal/)
2. 🔑 **Translated English text Gemini API Key**
3. 💻 Translated English text **Google Colab** Translated English text
4. 🧪 Translated English text API Key Translated English text

---

## Slide 6: 🔑 Translated English text Gemini API Key (Step-by-Step)

1. Translated English text **[aistudio.google.com](https://aistudio.google.com)**
2. Login Translated English text Google Account
3. Translated English text **"Get API Key"** (Translated English text)
4. Translated English text **"Create API Key"**
5. Translated English text Project → **Create API key in new project**
6. **Copy** API Key Translated English text (Translated English text!)

> ⚠️ Free tier: **15 RPM** (requests/minute) — Translated English text workshop

---

## Slide 7: 🔒 Translated English text API Key Translated English text Colab Secrets

1. Translated English text Google Colab
2. Translated English text 🔑 **Translated English text** (Translated English text) → "Secrets"
3. Translated English text **"Add new secret"**
4. Name: `GOOGLE_API_KEY`
5. Value: Translated English text API Key Translated English text copy Translated English text
6. Translated English text toggle **"Notebook access"** ✅

> 🎯 Translated English text — Translated English text notebook

---

## Slide 8: 🚨 Error 429 — Rate Limit Translated English text?

```
google.api_core.exceptions.ResourceExhausted: 429
You exceeded your current quota
```

**Translated English text:** Translated English text request Translated English text/Translated English text

### Free Tier Limits (Gemini 2.5 Flash):
| Limit              | Translated English text        |
| ------------------ | --------- |
| RPM (Requests/min) | 15        |
| TPM (Tokens/min)   | 1,000,000 |
| RPD (Requests/day) | 1,500     |

---

## Slide 9: 💡 Translated English text Error 429

### Translated English text:
1. **Translated English text 1-2 Translated English text** Translated English text run Translated English text
2. **Translated English text run cell Translated English text** — Translated English text output Translated English text

### Translated English text (Translated English text):
3. Translated English text **retry + sleep** Translated English text:
```python
import time
for attempt in range(3):
    try:
        response = client.models.generate_content(...)
        break
    except Exception as e:
        if '429' in str(e):
            print(f'⏳ Rate limit, Translated English text {30*(attempt+1)} Translated English text...')
            time.sleep(30 * (attempt + 1))
        else:
            raise
```

---

## Slide 10: 🧪 Translated English text Colab → Translated English text notebook Translated English text → Run:

```python
# 1. Translated English text API Key
from google.colab import userdata
import os
os.environ['GOOGLE_API_KEY'] = userdata.get('GOOGLE_API_KEY')

# 2. Translated English text
from google import genai
client = genai.Client(api_key=os.environ['GOOGLE_API_KEY'])
resp = client.models.generate_content(
    model='gemini-2.5-flash',
    contents='Translated English text 1 Translated English text'
)
print(f'✅ Translated English text: {resp.text}')
```

Translated English text ✅ = Translated English text!

---

## Slide 11: 📋 Checklist Translated English text

- [ ] Translated English text [myhero.megawiz.co.th/student-portal](https://myhero.megawiz.co.th/student-portal/) Translated English text
- [ ] Translated English text Google Account
- [ ] Translated English text Gemini API Key Translated English text
- [ ] Translated English text Key Translated English text Colab Secrets Translated English text
- [ ] Run Translated English text → Translated English text ✅

> 🎯 **Translated English text checklist Translated English text → Translated English text workshop Translated English text!**

---

## Slide 12: 🏆 Certificate

Translated English text workshop Translated English text:
- Translated English textpointsTranslated English text (AI Grading)
- Translated English text **Certificate** Translated English text [myhero.megawiz.co.th](https://myhero.megawiz.co.th/student-portal/)
- Translated English text (PDF)

---

## Slide 13: ❓ Translated English text?

| Translated English text              | Translated English text                                   |
| ----------------- | -------------------------------------- |
| Translated English text myhero Translated English text   | Translated English text spam / Translated English text                 |
| Translated English text OTP        | Translated English text spam folder / Translated English text 1 Translated English text             |
| API key not valid | Translated English text key Translated English text aistudio.google.com      |
| Error 429         | Translated English text 1-2 Translated English text                   |
| Colab Translated English text          | Runtime → Change runtime type → T4 GPU |

- Translated English text / TA Translated English text
