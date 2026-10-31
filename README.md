# Supercart Partner (Android WebView app)

Wraps https://supercart-iota.vercel.app/delivery/signup in an Android app.
When the website asks for location, the standard Android "Allow / Don't allow" dialog appears.
If the user taps Allow, the site gets the location; if Deny, the site gets an error.

## APK banane ke 2 tareeke

### A) Phone se, GitHub ke through (computer nahi chahiye)
1. github.com par naya repository banao.
2. Is folder ki saari files upload karo (`.github` folder samet).
3. Repo me **Actions -> Build APK -> Run workflow** dabao.
4. 4-5 minute baad run me **supercart-partner-apk** artifact download karo. Usme `app-debug.apk` hogi.
5. Phone me APK install karo (Settings me "Install unknown apps" allow karna padega).

### B) Computer par Android Studio se
1. Android Studio me **Open** -> is folder ko chuno.
2. Gradle sync hone do.
3. **Build -> Build APK(s)**.

## Notes
- Ye debug-signed APK hai. Install karne ke liye theek hai. Play Store ke liye release signing key banani hogi.
- Website ka link badalna ho to `MainActivity.java` me `START_URL` aur `ALLOWED_HOST` badlo.
- Location kaam karne ke liye phone ka GPS/Location ON hona chahiye.
- `icon-512.png` Play Store listing ke liye hai.
