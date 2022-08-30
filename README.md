<a href="https://flutter.dev/">
  <h1 align="center">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://storage.googleapis.com/cms-storage-bucket/6e19fee6b47b36ca613f.png">
      <img alt="Flutter" src="https://storage.googleapis.com/cms-storage-bucket/c823e53b3a1a7b0d36a9.png">
    </picture>
  </h1>
</a>

# Belajar Flutter

## Apa itu Flutter?
<p align="justify">
  Flutter adalah SDK (Software Development Kit) yang dikembangkan oleh Google untuk membuat aplikasi yang bagus dan bisa berjalan pada berbagai platform. Flutter 2 yang merupakan versi terbaru memberikan dukungan pada Anda untuk membangun aplikasi pada sistem operasi Android, iOS, Web, Windows, Linux, dan MacOS. Dengan ini, Anda cukup sekali coding atau dikenal dengan single codebase. Flutter juga sudah digunakan oleh banyak developer maupun organisasi di seluruh dunia, selain itu Flutter bersifat open source.
</p>

## Instalasi Flutter
1. Unduh paket instalasi untuk mendapatkan versi stabil terbaru dari Flutter SDK di alamat web https://flutter.dev/docs/development/tools/sdk/releases. Ambil versi terbaru pada stable channel sesuai sistem operasi yang digunakan.
2. Ekstrak berkas zip dan tempatkan folder flutter pada lokasi instalasi yang diinginkan untuk Flutter SDK. Misalnya C:\Development, jangan pasang Flutter di direktori seperti C:\Program Files atau yang membutuhkan hak istimewa seperti administrator.
3. Temukan berkas flutter_console.bat di dalam direktori flutter tersebut. Mulai dengan klik dua kali atau jalankan script tersebut dan Anda sekarang siap untuk menjalankan perintah Flutter di Flutter Console.
4. Dari bar pencarian di Start menu, ketik ‘env’ dan pilih Edit Environment Variable untuk akun Anda.
5. Klik pada tombol Environment Variables.
6. Di bawah User variabel periksa apakah ada entri yang disebut PATH, jika ada maka pilih lalu edit, jika tidak ada maka buat baru dengan nama variabel Path.
7. Edit atau tambahkan value-nya dengan direktori Flutter SDK.
- Jika terdapat entri, tambahkan path lengkap ke flutter\bin menggunakan tanda titik koma (;) sebagai pemisah dari nilai yang ada (jika menggunakan mode edit satu baris).
- Jika entri tidak ditemukan, buat user variabel baru dan beri nama Path dan beri nilai flutter\bin sebagai nilainya.
8. Perhatikan bahwa Anda harus menutup dan membuka kembali semua jendela konsol yang ada agar perubahan dapat terlihat.
9. Flutter doctor adalah perintah untuk mengecek kelengkapan framework flutter yang Anda gunakan, seperti versi flutter yang digunakan, Android SDK yang digunakan, iOS SDK yang digunakan (hanya pada MacOS), perangkat yang sudah terhubung, dan semacamnya.  Periksa kembali dan pastikan dependensi untuk pengaturan sudah lengkap. Jalankan perintah berikut untuk membuka flutter doctor:
```
flutter doctor
```

## Instalasi IDE
#### 1. Android Studio/IntelliJ
Android Studio dan IntelliJ menawarkan pengalaman IDE yang terintegrasi lengkap dengan plugin khusus untuk Flutter. Untuk mengunduh Android Studio, Anda dapat mengunjungi tautan https://developer.android.com/studio. Sedangkan jika Anda memilih IntelliJ maka dapat melalui tautan https://www.jetbrains.com/idea/download/.

Berikut adalah cara instalasi Flutter danplugin Dart di Android Studio/IntelliJ:
1. Pertama, buka terlebih dahulu Android Studio/IntelliJ.
2. Pada halaman Welcome pilih menu Plugins di bagian kiri.
3. Jika IDE Android Studio/IntelliJ tidak pad ahalaman Welcome, Anda dapat pilih menu File > Settings > Plugins bagi pengguna OS Windows dan Linux. Sedangkan bagi pengguna MacOS, Pilih menu Android Studio > Preferences > Plugins.
4. Pilih menu Marketplace, ketik Flutter pada pencarian plugins dan instal. Saat Anda melakukan instalasi plugins Flutter maka secara otomatis Dart juga terinstal.
5. Klik Restart saat diminta. Jika tidak muncul, silakan muat ulang secara manual aplikasi Android Studio/IntelliJ.

#### 2. Visual Studio Code
Visual Studio Code (VSCode) adalah editor ringan untuk mengkombinasikan baris perintah khususnya aplikasi Flutter dan dilengkapi dukungan debugging. Untuk mengunduh Visual Studio Code, kunjungi tautan https://code.visualstudio.com/download.

Berikut adalah cara instalasi plugin Flutter dan Dart di VSCode:
1. Buka aplikasi Visual Studio Code yang telah diinstal sebelumnya.
2. Kemudian aktifkan Command Line dengan cara pilih View > Command Pallete…
3. Ketik “Install” lalu pilih Extensions: Install Extensions. Atau langsung klik pada tab Extensions yang ada pada bagian kiri.
4. Ketik “Flutter” pada bidang pencarian Extensions, dan pilih Flutter dalam daftar ekstensi yang tersedia. Kemudian klik tombol Install. Secara otomatis plugin Dart juga akan terinstal.
5. Klik Reload to Activate untuk memuat ulang VSCode.
6. Aktifkan Command Line dengan cara pilih View>Command Pallete…
7. Ketik “doctor”, lalu pilih Flutter: Run Flutter Doctor.
8. Tinjau panel OUTPUT untuk melihat masalah apapun.

## Project Wizard
#### 1. Android Studio/IntelliJ
1. Buka Android Studio/IntelliJ.
2. Pilih New Flutter Project.
3. Pilih Flutter SDK path yang tersedia. Jika path tidak tersedia, klik tombol titik tiga untuk cari direktori Flutter SDK. Kemudian klik tombol Next.
4. Masukkan nama proyek yang ingin dibuat pada Project name. Tentukan di mana proyek Anda disimpan pada Project location. Deskripsikan proyek Anda pada kolom Descriptions. Pilih Application pada kolom Project type untuk membuat aplikasi Flutter. Masukkan nama domain yang ingin dibuat pada Organization. Pilih Kotlin untuk membuat proyek Android-nya menggunakan bahasa Kotlin dan Swift untuk membuat proyek iOS-nya menggunakan bahasa Swift.
5. Centang Platform yang ingin dikembangkan saat proyek Flutter dibuat, misal Anda ingin mengembangkan platform Android dan iOS, centang hanya keduanya saja. Selanjutnya, centang pada Create project offline jika Anda ingin membuat proyek dapat diakses ketika sedang offline. Klik Finish.
6. Tunggu beberapa saat hingga Android Studio selesai membuat project.

#### 2. Visual Studio Code
1. Buka Visual Studio Code.
2. Aktifkan Command Line dengan cara klik View>Command Pallete…
3. Ketik “Flutter” lalu pilih Flutter: New Project.
4. Pilih flutter application, lalu tentukan path to project.
5. Masukkan nama project, dan tekan Enter.
6. Tunggu beberapa saat sampai VSCode selesai menyiapkan project.

## Menjalankan Emulator
#### 1. Android Emulator
1. Untuk menjalankan aplikasi, klik menu Tools, lalu pilih Device Manager.
2. Untuk membuat emulator baru, klik tombol Create device atau Create virtual device.
3. Halaman Select Hardware akan muncul. Jika Anda ingin membuat spesifikasi hardware (perangkat keras) sendiri, pilih New Hardware Profile. Anda dapat menentukan konfigurasi hardware sesuai dengan kebutuhan Anda. Ingatlah untuk menggunakan konfigurasi emulator yang sesuai dengan kemampuan laptop atau komputer yang Anda gunakan. Setelah itu klik Next.
4. Halaman System Image akan muncul.
Pada halaman ini Anda dapat memilih versi Android dari emulator yang akan Anda buat. Pilih versi yang sudah diunduh, misal Pie. Lihat tombol download di sebelah kanan. Anda perlu mengunduh terlebih dahulu jika ingin menggunakannya. Setelah itu klik Next.
5. Halaman Verify Configuration akan muncul.
Pada halaman ini Anda bisa mengubah konfigurasi hardware yang telah ditentukan sebelumnya. Tekan tombol Show Advanced Setting pada bagian kiri bawah. Jika sudah selesai, klik Finish. Pengaturan emulator sudah selesai dan bisa langsung dijalankan. Anda dapat membuka emulatornya dengan menekan tombol hijau yang ada di sebelah kanan.

#### 2. Android Device
1. Pastikan peranti yang akan dipakai sesuai dengan target SDK atau paling tidak mendukung versi SDK terendah yang digunakan aplikasi.
2. Buka setting dan masuk ke dalam menu About. Pada halaman menu ini, Anda perlu menemukan informasi tentang Build number.
3. Kemudian tekan Build number sebanyak 7 kali.
4. Kembali ke menu setting di awal dan akan muncul menu baru di bawah about yaitu Developer Options.
5. Masuk ke dalam menu Developer Options dan pastikan opsi USB Debugging Mode sudah dalam keadaan On.
6. Setelah menyelesaikan pengaturan pada peranti, peranti pun dapat dihubungkan dengan laptop atau komputer yang Anda pakai.

## Menjalankan Project Flutter
#### 1. Android Studio/IntelliJ
1. Pada target selector, pilih perangkat Android untuk menjalankan aplikasi. Jika tidak ada yang terdaftar, pilih Tools > Device Manager dan buat satu emulator di Device Manager.
2. Klik ikon run pada toolbar, atau buka item menu Run > Run ‘main.dart’.
3. Setelah build aplikasi selesai, Anda akan melihat aplikasi starter di perangkat Anda.

#### 2. Visual Studio Code
1. Pilih perangkat di area Device Selector.
- Jika tidak ada perangkat yang tersedia dan Anda ingin menggunakan simulator perangkat, klik No Device dan luncurkan simulator.
- Untuk menyiapkan perangkat fisik (smartphone pribadi), ikuti petunjuk khusus perangkat pada saat melakukan Install Flutter SDK untuk OS Anda.
2. Aktifkan Command Line dengan cara pilih Run > Start Debugging atau tekan F5, atau pada kode void main akan muncul run dan debug, atau pada tab Run di bagian kiri.
3. Tunggu hingga aplikasi diluncurkan dan lihat progress dalam tampilan Debug Console.
4. Setelah build aplikasi selesai, Anda akan melihat aplikasi starter di perangkat Anda.

## Menjalankan di Web
<p align="justify">
Selain platform mobile, Flutter juga bisa berjalan pada web browser. Dalam proses pengembangan, untuk keperluan debugging kita perlu menggunakan Google Chrome sebagai browser. Sejak Flutter versi 2.0 Flutter Web sudah memasuki versi stable sehingga bisa digunakan secara langsung. Jika menggunakan versi di bawahnya, Anda perlu mengaktifkan channel beta terlebih dahulu. Silakan ikuti langkahnya pada blog berikut.
</p>
<p align="justify">
Untuk menambahkan dukungan web pada project Anda, jalankan perintah berikut melalui terminal dari lokasi project:
</p>

```
flutter config --enable-web
flutter create .
```

<p align="justify">
Setelah konfigurasi dan proses re-create berhasil, folder web akan ditambahkan ke dalam folder project Anda. Di dalam folder ini akan berisi berkas html dan konfigurasi web lainnya. Anda bisa mencoba menjalankan aplikasi web Flutter ini dengan memilih target device chrome pada IDE yang Anda gunakan. Ketika target device Chrome sudah terpilih seperti di atas, Anda dapat menjalankan aplikasi dengan cara yang sama seperti ketika menjalankannya pada platform mobile. Jika Anda ingin menjalankan melalui terminal, maka perintahnya adalah seperti ini:
</p>

```
flutter run -d chrome
```
Setelah proses build selesai, jendela browser akan muncul dan menampilkan aplikasi Anda.
Pada Flutter Web, perlu diperhatikan bahwa Flutter memiliki dua jenis renderer yang berbeda, keduanya antara lain:
- HTML renderer : 
Renderer ini menggunakan kombinasi elemen HTML, CSS, Canvas, dan SVG. Jenis renderer ini memiliki ukuran unduhan yang lebih kecil.
- CanvasKit renderer : 
Renderer ini bekerja dengan cara yang sama dengan platform mobile atau desktop. CanvasKit renderer memiliki performa yang lebih tinggi, tetapi akan menambahkan ukuran hingga sekitar 2 MB.
Anda dapat menentukan renderer yang digunakan dengan menambahkan parameter pada command line, contohnya seperti berikut:

```
flutter run -d chrome --web-renderer html
flutter run -d chrome --web-renderer canvaskit
```

<p align="justify">
Jika Anda tidak mendefinisikan parameter --web-renderer, maka renderer akan menggunakan mode auto (default). Opsi ini akan menggunakan HTML renderer ketika aplikasi berjalan di browser mobile dan menggunakan CanvasKit saat aplikasi berjalan di browser desktop.
</p>

## Build APK
<p align="justify">
Sebelum mem-build APK, kita akan mengatur berkas android/app/src/main/AndroidManifest.xml. AndroidManifest.xml merupakan sebuah berkas yang berisikan informasi mengenai aplikasi Android yang akan di-build. Informasi-informasi tersebut berupa nama aplikasi, ikon, permission, screen orientation, dan lain-lain. Untuk mengatur nama aplikasi, kita cukup mengubah properti android:label yang ada pada file AndroidManifest.xml Isikan android:label dengan nama aplikasi yang diinginkan. Secara default ikon aplikasi Flutter kita adalah ikon Flutter. Untuk mengubah icon aplikasi dengan mudah, kita akan mengganti gambar ic_launcher.png yang berada pada folder android/app/src/main/res/ yang terbagi menjadi berbagai mipmap (ukuran resolusi ikon). Ketika aplikasi dalam mode debug atau profil, perizinan internet akan secara otomatis ditambahkan. Namun ketika Anda ingin menjalankan atau membuatnya dalam mode rilis, Anda perlu menambahkan semua perizinan yang dibutuhkan pada AndroidManifest. Untuk menambahkan perizinan pada aplikasi Android, Anda bisa menambahkan tag uses-permission pada AndroidManifest, di dalam tag manifest dan sejajar tag application. 
</p>

<p align="justify">
Setelah kita mengatur nama dan ikon aplikasi, langkah selanjutnya adalah melakukan build aplikasi menjadi APK. Sebelumnya terdapat tiga (3) jenis mode aplikasi yang perlu diketahui, yaitu debug, profile, dan release. APK debug umumnya digunakan untuk pengujian dan penggunaan aplikasi secara internal. Mode debug digunakan secara default ketika menjalankan aplikasi menggunakan perintah flutter run. Sementara untuk bisa dirilis melalui Google Play Store, Anda perlu membuat APK release. Sedangkan mode profile sama hal nya dengan release hanya saja tetap dapat di-debug menggunakan tools seperti DevTools dan tidak dapat dijalankan di emulator atau simulator. Pada kelas ini kita akan mempelajari bagaimana membuat APK debug. Caranya ialah menggunakan terminal pada Android Studio. Tekan tombol Terminal yang ada pada pojok kiri bawah. Bila menggunakan Visual Studio Code pilih menu terminal yang ada pada menu kiri atas. Lalu pilih new terminal. Jika terminal telah muncul, tuliskan perintah berikut:
</p>

```
flutter build apk --debug
```

<p align="justify">
Tunggu hingga proses build berhasil. Setelah berhasil, hasil build yang berupa berkas apk-debug.apk akan terletak di folder build/app/outputs/apk/debug/ atau akan muncul direktori tempat tersimpannya berkas ketika proses build selesai pada Terminal. Untuk bisa mem-build apk release dan mengunggahnya melalui Google Play Store, Anda memerlukan signing key. Signing key ini digunakan sebagai tanda tangan supaya aplikasi Anda lebih aman. Secara default Flutter menggunakan debug key sebagai signing key sehingga Anda sebenarnya bisa membuat apk release dengan menjalankan perintah berikut:
</p>

```
flutter build apk
```

<p align="justify">
Namun, tentunya akan lebih baik jika Anda menggunakan signing key milik Anda sendiri. Cara untuk membuat signing key dan membuat apk release dapat Anda baca pada tautan dokumentasi berikut: https://flutter.dev/docs/deployment/android.
</p>

## Build IPA
<p style="color:red; background-color:tomato; text-align:justify;">
Catatan: Build .IPA hanya bisa dijalankan dengan mendaftar akun Apple Developer Program. Silakan baca informasi tentang Apple Developer Program di sini https://developer.apple.com/programs/.
</p>
<p align="justify">
Pada materi ini kita akan mempelajari bagaimana melakukan build aplikasi Flutter menjadi berkas .ipa yang dapat dijalankan pada perangkat iOS. Sebelum melakukan build, ada beberapa hal yang perlu kita atur seperti nama dan ikon aplikasi.
</p>

<p align="justify">
Untuk mengatur nama aplikasi buka berkas Info.plist pada direktori /ios/Runner/. Konfigurasi untuk nama aplikasi dapat Anda temukan dan ubah pada key Bundle Name. Sama seperti perangkat Android, layar untuk perangkat iPhone juga terbagi ke dalam berbagai ukuran. Sehingga diperlukan juga ukuran ikon yang berbeda. Selanjutnya Anda dapat mengganti folder Assets.xcassets yang ada pada direktori /ios/Runner/ dengan hasil ikon yang sudah Anda generate. File IPA juga terbagi menjadi debug, profile, dan release. Namun untuk melakukan build aplikasi Flutter menjadi IPA hanya bisa dilakukan pada device macOS. Untuk melakukan build aplikasi menjadi .ipa Anda cukup membuka terminal pada editor atau IDE Anda lalu menjalankan perintah berikut:
</p>

```
flutter build ios
```

<p align="justify">
Secara default perintah di atas akan menghasilkan ipa release, sedangkan jika Anda ingin membuat versi debug atau profile, gunakan perintah:
</p>

```
flutter build ios --debug
```

<p align="justify">
Namun, bagi Anda yang tidak mempunyai perangkat Apple jangan khawatir, Anda tetap dapat men-deploy project Anda ke iOS menggunakan CI/CD seperti Codemagic dan Bitrise.
</p>

## Web Deployment
<p align="justify">
Untuk mengatur nama aplikasi, kita bisa membuka berkas manifest.json. Konfigurasi untuk nama aplikasi dapat Anda temukan dan ubah pada key name dan short_name. Platform web juga membutuhkan icon dalam berbagai ukuran. Icon untuk web dapat Anda taruh pada folder /web/icons. Kemudian, Anda perlu mendaftarkannya pada berkas manifest.json. Sama seperti build aplikasi android dan ios, untuk mem-build aplikasi Flutter web kita menjalankan perintah flutter web. Perintah selengkapnya adalah seperti ini:
</p>

```
flutter build web
```

<p align="justify">
Sama seperti ketika menjalankan flutter web, ketika melakukan build, kita juga bisa menentukan renderer yang ingin digunakan. Untuk menentukan renderer yang digunakan, tambahkan parameter --web-renderer pada perintah flutter build. Jika tidak mendefinisikan parameter --web-renderer maka mode auto yang akan digunakan. Hasil build akan Anda temukan pada folder /build/web. Folder inilah yang nantinya bisa Anda deploy ke sebuah web hosting atau web server.
</p>