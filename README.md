![](.github/images/jukebox.png)
# Jukebox
> Just a simple Discord music bot

<a href='https://discordapp.com/oauth2/authorize?client_id=698573904129818624&permissions=53857345&scope=bot'><img src="https://img.shields.io/static/v1?label=Invite%20Me&message=Jukebox%239319&plastic&color=7289DA&logo=discord"></a>
<a href='https://hub.docker.com/r/hazmi35/jukebox' alt="Available on Docker Hub"><img src="https://badgen.net/docker/size/hazmi35/jukebox/latest/amd64"></a>
<a href='https://github.com/Hazmi35/jukebox/actions?query=workflow%3A%22Lint+code+%26+compile+test%22'><img src='https://github.com/Hazmi35/jukebox/workflows/Lint%20code%20&%20compile%20test/badge.svg' alt='CI Status' /></a>
<img src="https://badgen.net/badge/icon/typescript?icon=typescript&label">
<a href="https://heroku.com/deploy"><img src="https://www.herokucdn.com/deploy/button.svg" alt="Deploy"></a>

## Usage

**[⚠] Requires [Node.JS](https://nodejs.org) version 16.6.0 or above.**

1. Install [Node.JS](https://nodejs.org)
2. Install requirements for yt-dlp

   For Linux/Mac OS/Unix-like system, install [Python 3](https://www.python.org/downloads/), and add them to the PATH environment variable

   For Windows, you don't need to install Python, but you need to install [Microsoft Visual C++ 2010 Service Pack 1 Redistributable Package (x86)](https://download.microsoft.com/download/1/6/5/165255E7-1014-4D0A-B094-B6A430A6BFFC/vcredist_x86.exe)

3. Rename `.env.schema` to `.env` and fill out the values (example on .env.example)
4. Install dependencies as stated [here](https://github.com/Hazmi35/jukebox#install)
5. Run `npm run build`
6. (Optional) Prune dev dependencies (This is good to save disk spaces):
```sh
$ npm prune --production
```
1. Start it with `npm start`. And you're done!

Notes: 
1. You only need to configure .env file when you're using the [Docker image](https://github.com/Hazmi35/jukebox#Docker)
2. If you're using "Deploy to Heroku" button, you don't need to do this.

## Install

Without optional packages
```sh
$ npm install --no-optional
```

With optional packages (Recommended)

```sh
$ npm install
```
For optional packages, you need to install build tools as stated [here](https://github.com/nodejs/node-gyp#installation) and you also need to install [Git](https://git-scm.com/)

## Docker
Want to use Dockerized version of jukebox? sure! we provide them on the [Docker Hub](https://hub.docker.com/r/hazmi35/jukebox) and also in [GitHub Container Registry](https://github.com/users/Hazmi35/packages/container/package/jukebox)

### Volumes
[Docker Volumes](https://docs.docker.com/storage/volumes/) are needed to store cache and logs persistently

### Example:
```sh
$ docker run --env-file .env --volume cache:/app/cache --volume logs:/app/logs --restart unless-stopped hazmi35/jukebox
```
We also provide [docker-compose.yml](docker-compose.yml) if you want to go that way

### Compose Example
```sh
$ docker-compose up
```

## Features
- A production-ready music bot, suitable for you that dislike hassling with the code.
- Basic Commands (Help, Ping, Invite & Eval [for advanced bot owners])
- Basic Music Commands (Play, Skip, Stop, Pause & Resume, Now Playing, Queue, Repeat, Volume)
- Caching! (cache youtube downloads)
- Configurable
- Docker-friendly
- Lightweight (only around 120MB with dev dependencies pruned)

## Penggunaan

**[⚠] Membutuhkan [Node.JS](https://nodejs.org) versi 16.6.0 atau lebih tinggi.**

1. Instal [Node.JS](https://nodejs.org)
2. Persyaratan instal untuk yt-dlp

   Untuk sistem mirip Linux/Mac OS/Unix, instal [Python 3](https://www.python.org/downloads/), dan tambahkan ke variabel lingkungan PATH

   Untuk Windows, Anda tidak perlu menginstal Python, tetapi Anda perlu menginstal [Microsoft Visual C++ 2010 Service Pack 1 Redistributable Package (x86)](https://download.microsoft.com/download/1/6/5/ 165255E7-1014-4D0A-B094-B6A430A6BFFC/vcredist_x86.exe)

3. Ganti nama `.env.schema` menjadi `.env` dan isi nilainya (contoh pada .env.example)
4. Instal dependensi seperti yang dinyatakan [di sini](https://github.com/Hazmi35/jukebox#install)
5. Jalankan `npm run build`
6. (Opsional) Pangkas dependensi dev (Ini bagus untuk menghemat ruang disk):
```sh
$npm memangkas --produksi
```
1. Mulai dengan `npm start`. Dan Anda sudah selesai!

Catatan:
1. Anda hanya perlu mengonfigurasi file .env saat menggunakan [gambar Docker](https://github.com/Hazmi35/jukebox#Docker)
2. Jika Anda menggunakan tombol "Deploy to Heroku", Anda tidak perlu melakukan ini.

## Install

Tanpa paket opsional
```sh
$npm install --no-opsional
```

Dengan paket opsional (Disarankan)

```sh
$npm instal
```
Untuk paket opsional, Anda perlu menginstal alat build seperti yang dinyatakan [di sini](https://github.com/nodejs/node-gyp#installation) dan Anda juga perlu menginstal [Git](https://git-scm. com/)

## buruh pelabuhan
Ingin menggunakan jukebox versi Dockerized? Tentu! kami menyediakannya di [Docker Hub](https://hub.docker.com/r/hazmi35/jukebox) dan juga di [GitHub Container Registry](https://github.com/users/Hazmi35/packages/container /paket/jukebox)

### Volume
[Volume Docker](https://docs.docker.com/storage/volumes/) diperlukan untuk menyimpan cache dan log secara terus-menerus

### Contoh:
```sh
$ docker run --env-file .env --volume cache:/app/cache --volume logs:/app/logs --restart kecuali hazmi35/jukebox dihentikan
```
Kami juga menyediakan [docker-compose.yml](docker-compose.yml) jika Anda ingin melakukannya

### Tulis Contoh
```sh
$ komposisi buruh pelabuhan
```

## Fitur
- Bot musik siap produksi, cocok untuk Anda yang tidak suka mengganggu kode.
- Perintah Dasar (Bantuan, Ping, Undang & Evaluasi [untuk pemilik bot tingkat lanjut])
- Perintah Musik Dasar (Play, Skip, Stop, Pause & Resume, Now Playing, Queue, Repeat, Volume)
- Caching! (cache unduhan youtube)
- Dapat dikonfigurasi
- Ramah buruh pelabuhan
- Ringan (hanya sekitar 120MB dengan dependensi dev dipangkas)
