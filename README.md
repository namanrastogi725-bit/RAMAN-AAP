# RAMAN — Phone par Install Karne Ka Tarika

Ye ek **PWA (Progressive Web App)** hai — asli Play Store APK nahi, lekin phone ke
home screen par install ho kar bilkul app jaisi chalti hai (apna icon, full-screen,
offline bhi kaam karti hai).

## Zaroori: Pehle host karo (1 baar, free)

Browser directly folder nahi khol sakta jaisे real app; isliye pehle inhe kisi free
static hosting par daalo — 2 minute ka kaam hai:

### Option A — Netlify Drop (sabse aasan, sign-up bhi nahi chahiye)
1. Browser mein kholo: https://app.netlify.com/drop
2. Is poore `tape-app` folder ko wahan drag-and-drop karo
3. Aapko ek link milega jaise `https://xyz123.netlify.app`

### Option B — GitHub Pages
1. Ek naya GitHub repo banao, ye saari files upload karo
2. Repo Settings → Pages → source ko `main` branch set karo
3. Kuch minute mein link mil jayega

## Phone par install karna (Android)

1. Upar wala link apne phone ke **Chrome** browser mein kholo
2. Chrome menu (⋮) kholo → **"Add to Home screen"** / **"Install app"** dabao
3. RAMAN ka icon home screen par aa jayega — usse tap karke kholo, ye
   full-screen app jaisi chalegi (address bar bhi nahi dikhegi)

iPhone par: Safari mein link kholo → Share button → **"Add to Home Screen"**

## Isme kya hai
- Naya polished icon (uptrend sparkline + "R" wordmark) aur social share thumbnail
- Live, Trending, Search, Analyse tabs
- Phone number + OTP login (demo — real SMS nahi jaata)
- Paper trading (virtual paisa) + Buy/Sell history
- Auto-refresh, Auto-analyse-all, Auto-pick profit picks
- Broker/API settings screen (real trading ke liye backend chahiye)

## Real APK chahiye ho to
Agar aapko Play Store wali asli `.apk` file chahiye, uske liye ye extra steps
lagenge (ye main abhi nahi kar sakta kyunki mujhe Android build tools/internet
access nahi hai is jagah se):
1. Node.js + Android Studio install karo apne computer par
2. Is web app ko **Capacitor** (`npm install @capacitor/core @capacitor/cli`) se
   wrap karo — ye web app ko native Android project mein badal deta hai
3. Android Studio se APK build/sign karo

Agar chaho to main aapko Capacitor ke liye config files bana ke de sakta hoon,
lekin final `.apk` compile karna aapko apne computer par karna hoga.
