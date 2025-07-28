# People Walking Counter

A lightweight real-time people counter built using **HTML**, **JavaScript**, and **TensorFlow\.js**.\
This app detects and counts walking people from a live camera or uploaded video using the pre-trained **COCO-SSD** model.

---

## Features

- Real-time human detection using webcam or uploaded video
- Dynamic camera source selection
- Powered by TensorFlow\.js + COCO-SSD
- Object tracking with unique ID per person
- No backend needed – runs entirely in browser

---

## How It Works

1. Loads the `coco-ssd` model via TensorFlow\.js.
2. Detects objects on each video frame.
3. Filters for objects labeled as `"person"` with confidence > 0.6.
4. Tracks people using centroid distance comparison across frames.
5. Displays a bounding box and ID, and increments the total count.

---

## Getting Started

### Online Use

Just open the `index.html` file in a modern browser (Chrome recommended).

### Local Use

1. Clone the repository:

   ```bash
   git clone https://github.com/app-xcode/people-walking-counter.git
   cd people-walking-counter
   ```

2. Open `index.html` in your browser.

> No installation required. All dependencies are loaded from CDN.

---

## Project Structure

```
.
├── index.html         # Main application file
└── README.md          # Project description
```

---

## Dependencies

- TensorFlow\.js
- COCO-SSD Model

CDN links used:

```html
<script src="https://cdn.jsdelivr.net/npm/@tensorflow/tfjs"></script>
<script src="https://cdn.jsdelivr.net/npm/@tensorflow-models/coco-ssd"></script>
```

---

## License

MIT License © 2025

---

## Author

Built by [Etwin](https://github.com/app-xcode)

