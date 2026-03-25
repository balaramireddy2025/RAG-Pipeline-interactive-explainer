# RAG Pipeline — Interactive Team Reference

An interactive, step-by-step visual explainer of the full Retrieval-Augmented Generation pipeline.

🔗 **Live site:** `https://<your-username>.github.io/<repo-name>/`

## What's Inside

| Step | Page | Interactive Feature |
|------|------|---------------------|
| 01 | What is RAG | Problem/Solution cards |
| 02 | Loading | Document type cards + code |
| 03 | Preprocessing | Cleaning pipeline + code |
| 04 | Chunking | **Live chunking demo** with 4 strategies + sliders |
| 05 | Embeddings | **Interactive 2D scatter plot** with hover tooltips |
| 06 | Vector Store | **Animated grid** — Store Chunks → Query → Reset |
| 07 | Retrieval | **Cosine similarity canvas** + live retrieval demo |
| 08 | Generation | **Step-by-step prompt builder** + LLM answer |

## Deploy to GitHub Pages (5 minutes)

### Option A — Automatic (GitHub Actions) ⭐ Recommended

1. Create a new GitHub repository (public or private with Pages enabled)
2. Push all files to the `main` branch:
   ```bash
   git init
   git add .
   git commit -m "feat: RAG pipeline interactive explainer"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
3. In your repo → **Settings → Pages**:
   - Source: **GitHub Actions**
4. The workflow runs automatically. Your site will be live at:
   `https://<your-username>.github.io/<repo-name>/`

### Option B — Manual (no Actions needed)

1. Push files to your repo
2. In **Settings → Pages**:
   - Source: **Deploy from a branch**
   - Branch: `main`, folder: `/ (root)`
3. Wait ~2 minutes → site is live

## Local Preview

```bash
# Python
python -m http.server 8080

# Node
npx serve .

# Then open http://localhost:8080
```

## Sharing With Your Team

Once deployed, share the URL:
```
https://<your-username>.github.io/<repo-name>/
```

No login required. Works on desktop and mobile.

## Customizing

- **Sample text**: Edit `SAMPLE` constant in the `<script>` section of `index.html`
- **Retrieval DB**: Edit the `RETRIEVAL_DB` array to use your own document excerpts
- **Colors**: Change CSS variables in `:root` at the top of the `<style>` section
- **Company name**: Search and replace "The company provides" with your own content
