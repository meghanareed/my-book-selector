# My Book Selector

My Book Selector is a user-friendly application designed to help you choose your next book based on various criteria. Whether you're looking for a specific genre, author, or publication date, this tool provides personalized recommendations to enhance your reading experience.

## Features
- **Genre-based recommendations**: Filter books by preferred genres.
- **Author searches**: Find books by specific authors.
- **Publication date filters**: Choose books based on their release dates.
- **User-friendly interface**: Easy navigation and seamless user experience.
- **Save your favorites**: Keep track of the books you love or want to read later.

## Getting Started
To get started, simply clone the repository and follow the instructions provided in the installation section. 

```bash
git clone https://github.com/meghanareed/my-book-selector.git
```

### Installation
1. Navigate to the project directory.
2. Install the required dependencies.

## Usage
Run the application from your terminal or preferred IDE and follow the prompts to get recommendations.

## Mascots

A reading buddy is drawn at random each time the app picks a book. The art lives
in `assets/mascots/` and the roster is one object in `my-book-selector.html`.

To add your own:

1. **Prepare the image.** A square PNG with a transparent background, 320x320.
   The modal is cream, so anything with a baked-in white or checkerboard
   background will show as a visible rectangle.
2. **Save it** as `assets/mascots/<name>.png`.
3. **Register it** in `MASCOT_IMG`:

   ```js
   const MASCOT_IMG = {
     penguin: 'assets/mascots/penguin.png',
     ...
     hedgehog: 'assets/mascots/hedgehog.png'
   };
   ```

4. **Give it lines** in `QUOTES`, using the same key:

   ```js
   hedgehog: ["Sharp choice!", "Curled up with this one all night."],
   ```

That's all — the random picker, the preloader and the speech bubble read from
those two objects, so nothing else needs changing. A buddy registered in
`MASCOT_IMG` without a matching `QUOTES` entry will throw when it comes up.

Keep the files small. They're all preloaded at startup so the first pick doesn't
flash an empty frame, and the current nine total about 170 KB. Quantising to a
128-colour palette shrinks this kind of flat cartoon art roughly 6x with no
visible difference.

## Contributing
We welcome contributions! Please see the [Contributing Guide](CONTRIBUTING.md) for more details.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.