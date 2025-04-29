# android-app-loja-online
Estudando Android Studio via app de loja online.

# Passos

### Arquivo build.gradle.kts (Project...) add Firebase:
alias(libs.plugins.google.gms.google.services) apply false

### Arquivo build.gradle.kts (Module...) add Firebase:
alias(libs.plugins.google.gms.google.services)

Depois de kotlinOptions add:
buildFeatures {
    viewBinding = true
}

Dentro de dependencies add:
implementation("com.github.bumptech.glide:glide:4.12.0")
implementation("com.google.code.gson:gson:2.9.1")
implementation("com.tbuonomo:dotsindicator:5.0")
implementation(libs.firebase.database)

### Arquivo libs.versions.toml add depois de constraintlayout:
googleGmsGoogleServices = "4.4.2"
firebaseDatabase = "21.0.0"

### Apertar Sync Now na barra azul superior

24:24