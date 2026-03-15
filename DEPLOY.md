# Deploy Denver Solar Site

## Option 1: GitHub Pages (recommended)
```bash
gh auth login
cd ~/.openclaw/workspace/denver-solar
gh repo create denver-solar --public --source=. --push
# Then go to repo Settings > Pages > Deploy from branch: main
# Site will be live at: https://<username>.github.io/denver-solar/
```

## Option 2: Netlify (drag & drop)
1. Go to https://app.netlify.com/drop
2. Drag the `denver-solar` folder onto the page
3. Done — instant URL

## Option 3: Surge.sh
```bash
cd ~/.openclaw/workspace/denver-solar
surge . denver-solar-case.surge.sh
# Creates account on first run (email + password)
```

## Option 4: Vercel
```bash
npx vercel --prod
# Follow prompts
```

## Preview locally
```bash
cd ~/.openclaw/workspace/denver-solar
python3 -m http.server 8888
# Open http://localhost:8888
```
