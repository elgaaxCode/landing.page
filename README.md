# 🛠️ Informasi Script

```plaintext
╔═════════════════════════════════╗
║ 🛠️ Informasi Script
╠═════════════════════════════════╣
║ 📦 Version    : 1.0
║ 👨‍💻 Developer  : ElgaaXcode
║ 🌐 Website    :
║ 💻 GitHub     :
╚═════════════════════════════════╝
```

```javascript
⚠️ Peringatan:
SCRIPT INI TIDAK BOLEH DIPERJUALBELIKAN.

```
## Menggunakan API

```javascript
const response = await api.get("/api/random/zikir");
```

## Menggunakan API dengan Parameter

```javascript
const response = await api.getBuffer("/api/maker/attp2", { text: content });
```
## Menggunakan API untuk upload media sementara

```javascript
const response = await api.tmpUpload(mediaPath);
```

# =======================

## Mengirim pesan teks

```javascript
await sock.sendMessage(remoteJid, { text: "Example" });
await sock.sendMessage(remoteJid, { text: "Example" }, { quoted: message });
```

## Mengirim gambar dari URL dan buffer

```javascript
await sock.sendMessage(remoteJid, {
  image: { url: "https://example.com/tes.jpg" },
caption: `Caption`,
});
await sock.sendMessage(
  remoteJid,
  { image: { url: "https://example.com/tes.jpg" }, caption: `Caption` },
  { quoted: message }
);

await sock.sendMessage(remoteJid, { image: buffer, caption: `Caption` });
await sock.sendMessage(
remoteJid,
  { image: buffer, caption: `Caption` },
  { quoted: message }
);
```

## Mengirim audio dari URL dan buffer

```javascript
await sock.sendMessage(
  remoteJid,
  { audio: { url: "" }, mimetype: "audio/mp4" },
  { quoted: message }
);
await sock.sendMessage(remoteJid, { audio: bufferAudio }, { quoted: message });
```
