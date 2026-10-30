ORDERS & RETURNS - ANDROID APP (Capacitor)

OPTION A: Bina Android Studio ke (GitHub se APK)
1. github.com par free account banao -> New repository (naam: orders-returns-app).
2. Is folder ki saari files (www, package.json, capacitor.config.json,
   .github folder, .gitignore) repository me upload karo
   (Add file -> Upload files; .github folder bhi upload karna zaroori hai).
3. Repository me "Actions" tab kholo -> "Build Android APK" -> Run workflow.
4. 5-8 minute baad run complete hoga. Run kholo -> neeche "Artifacts" me
   "orders-returns-apk" download karo -> zip kholo -> app-debug.apk.
5. APK ko phone me bhejo, install karo (Settings me "Install unknown apps" allow karna padega).

OPTION B: Android Studio / PC se
1. Node.js 20 aur JDK 17 install karo.
2. Is folder me terminal kholo:
     npm install
     npx cap add android
     npx cap sync android
     cd android
     ./gradlew assembleDebug        (Windows: gradlew.bat assembleDebug)
3. APK milegi: android/app/build/outputs/apk/debug/app-debug.apk

APP UPDATE KARNA HO: www/index.html edit karo, phir GitHub par push karo (ya Option B dobara chalao).

IMPORTANT: Data phone ke andar save hota hai. App uninstall karne ya
"Clear data" karne par records delete ho jayenge.
