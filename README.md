# 🏋️‍♀️ TreningsAppen - Mobilprogrammering ITF21019

## Om prosjektet

**TreningsAppen** er en Android-applikasjon utviklet som del av kurset ITF21019 Mobilprogrammering ved Høgskolen i Østfold. Appen er designet for å hjelpe brukere med å planlegge, spore og administrere sine treningsøkter på en enkel og effektiv måte.

### 👥 Utviklingsteam
- **Gruppe 15** - Høgskolen i Østfold
- **Kurs:** ITF21019 Mobilprogrammering
- **Utviklet av:** 
  - Daniel Nilsen Johansen
  - Marius Begby
  - Bharati Mainali

## ✨ Hovedfunksjoner

### 🎯 Treningsplanlegging
- Lag personlige treningsplaner
- Sett treningsmål og mål
- Planlegg økter i forveien

### 📊 Fremgangssporing
- Logg treningsøkter i sanntid
- Spor framgang over tid
- Visualiser treningsstatistikk

### 💪 Øvelsesdatabase
- Omfattende database med øvelser
- Detaljerte beskrivelser og instruksjoner
- Kategorisering etter muskelgrupper

### 🔥 Motivasjon & Utfordringer
- Personlige treningsutfordringer
- Fremgangsstatistikk og achievments
- Motiverende varsler og påminnelser

## 🛠️ Teknologier

### **Frontend**
- **Kotlin** - Moderne Android-utvikling
- **Android SDK** - Native Android-funksjoner
- **Jetpack Compose** - Moderne UI-toolkit
- **Material Design 3** - Google's designsystem

### **Backend & Database**
- **Firebase** - Google's backend-as-a-service
- **Firestore** - NoSQL cloud database
- **Firebase Authentication** - Brukerautentisering
- **Firebase Crashlytics** - Feilrapportering

### **Arkitektur**
- **MVVM Pattern** - Model-View-ViewModel
- **Repository Pattern** - Datahåndtering
- **LiveData & ViewModel** - Reaktiv programmering
- **Navigation Component** - App-navigasjon

## 📱 Systemkrav

### **Minimumskrav**
- **Android:** API level 27 (Android 8.1)
- **RAM:** 2GB
- **Lagring:** 100MB ledig plass
- **Internett:** Kreves for synkronisering

### **Anbefalt**
- **Android:** API level 33+ (Android 13+)
- **RAM:** 4GB+
- **Lagring:** 500MB ledig plass

## 🚀 Installasjon og Oppsett

### **Forutsetninger**
- **Android Studio** (Arctic Fox eller nyere)
- **JDK 11** eller nyere
- **Git** for versjonskontroll
- **Firebase-konto** for backend-tjenester

### **Steg-for-steg installasjon**

1. **Klon repositoryet**
   ```bash
   git clone https://github.com/Danieljoh98/TreningsAppen-ITF21019-Mobilprogrammering.git
   cd TreningsAppen-ITF21019-Mobilprogrammering-main
   ```

2. **Åpne i Android Studio**
   - Start Android Studio
   - Velg "Open an existing project"
   - Naviger til prosjektmappen

3. **Firebase-oppsett**
   - Opprett et Firebase-prosjekt på [Firebase Console](https://console.firebase.google.com/)
   - Legg til Android-app med package name: `hiof.gruppe15.treningsappen`
   - Last ned `google-services.json` og plasser i `app/` mappen

4. **Installer avhengigheter**
   ```bash
   ./gradlew build
   ```

5. **Kjør appen**
   - Koble til Android-enhet eller start emulator
   - Klikk "Run" i Android Studio

## 📁 Prosjektstruktur

```
app/src/main/java/hiof/gruppe15/treningsappen/
├── data/                    # Data layer
│   ├── repository/         # Repository classes
│   ├── datasource/         # Data sources (Firebase, local)
│   └── network/            # Network utilities
├── model/                   # Data models
│   ├── Exercise.kt         # Øvelse-modell
│   ├── Workout.kt          # Treningsøkt-modell
│   └── User.kt             # Bruker-modell
├── ui/                      # UI layer
│   ├── screens/            # Compose screens
│   ├── components/         # Reusable UI components
│   └── theme/              # App theme and styling
├── viewmodel/               # ViewModels
│   ├── WorkoutViewModel.kt
│   ├── ExerciseViewModel.kt
│   └── UserViewModel.kt
├── utils/                   # Utility classes
│   ├── Constants.kt
│   └── Extensions.kt
└── MainActivity.kt          # Main activity
```

## 🧪 Testing

### **Kjøre tester**
```bash
# Unit tester
./gradlew test

# Instrumenterte tester
./gradlew connectedAndroidTest

# UI-tester
./gradlew connectedDebugAndroidTest
```

### **Test Coverage**
- **Unit tests:** ViewModel og repository logic
- **Integration tests:** Firebase integration
- **UI tests:** Critical user flows

## 📱 Skjermbilder

*[Legg til skjermbilder av appen her når tilgjengelig]*

## 🚀 Deployment

### **Debug Build**
```bash
./gradlew assembleDebug
```

### **Release Build**
```bash
./gradlew assembleRelease
```

### **Firebase App Distribution**
```bash
./gradlew appDistributionUploadRelease
```

## 🤝 Bidrag til prosjektet

Vi ønsker bidrag velkommen! For å bidra:

1. **Fork** repositoryet
2. **Opprett** en feature branch (`git checkout -b feature/AmazingFeature`)
3. **Commit** endringene (`git commit -m 'Add some AmazingFeature'`)
4. **Push** til branchen (`git push origin feature/AmazingFeature`)
5. **Åpne** en Pull Request

## 📝 Kodestandard

- **Kotlin Coding Conventions**
- **Material Design Guidelines**
- **Android Architecture Guidelines**
- **Firebase Best Practices**

## 🐛 Kjente problemer

- [ ] Synkronisering kan ta litt tid på langsomme forbindelser
- [ ] Offline-modus under utvikling
- [ ] Push-varsler krever ytterligere konfigurasjon

## 🔮 Fremtidige funksjoner

- [ ] **Sosiale funksjoner** - Del treningsøkter med venner
- [ ] **AI-baserte anbefalinger** - Personlige treningsforslag
- [ ] **Wearable integration** - Smartwatch-støtte
- [ ] **Ernæringsplanlegging** - Kostholdsråd og -sporing
- [ ] **Video-instruksjoner** - Øvelsesvideo og tutorials

## 📞 Support og kontakt

**Utviklingsteam Gruppe 15:**
- **Daniel Nilsen Johansen** - danieljoh98@gmail.com - [@Danieljoh98](https://github.com/Danieljoh98)
- **Marius Begby** - [@mariusbegby](https://github.com/mariusbegby)
- **Bharati Mainali**
- **Kurs:** ITF21019 Mobilprogrammering, Høgskolen i Østfold

## 📄 Lisens

Dette prosjektet er utviklet som del av et studieprogram ved Høgskolen i Østfold.
For kommersielt bruk, kontakt utviklerne.

## 🙏 Takk til

- **Høgskolen i Østfold** - For utdanning og ressurser
- **Firebase** - For backend-infrastruktur
- **Material Design** - For designprinsipper
- **Android Community** - For åpen kildekode og ressurser

---

**Laget med ❤️ av Gruppe 15 - Daniel Nilsen Johansen, Marius Begby & Bharati Mainali**
**HiØF Mobilprogrammering ITF21019**