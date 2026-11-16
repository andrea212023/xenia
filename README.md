# Xenia

A card that opens for one mind only.

Xenia is a secret message card guarded by an alien bloom. The sender writes a message, a question, and the answer that opens it. The receiver meets a closed flower that flinches from touch, answers its question, then presses and holds while it opens and its glyphs resolve into the message.

## How it works

- **Grow a card:** write the message, the question, and the answer. You get a seed, a text code to send to your person.
- **Open a card:** paste the seed, answer the question, then press and hold the bloom.

## Privacy

The message is encrypted in the browser with AES-GCM. The key is derived from the answer with PBKDF2 (SHA-256, 200,000 iterations). Nothing is sent to a server. The lock is only as strong as the answer: a short or common answer can be guessed by anyone who holds the seed.

## Run it

The whole app is `index.html`. Open it over HTTPS or on localhost (browsers only allow the encryption API in a secure context), or publish the repository with GitHub Pages.

## Status

Prototype. The flora are drawn procedurally on a canvas.
