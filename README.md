# Marketing Landing Page

This project is a simple marketing landing page designed to showcase a product and drive sales. It includes a clean and responsive layout, styled with CSS and enhanced with JavaScript for interactivity.

## Project Structure

```
marketing-landing-page
├── src
│   ├── index.html       # Main HTML document for the landing page
│   ├── styles.css       # CSS styles for the landing page
│   └── main.js          # JavaScript for interactivity
├── package.json         # npm configuration file
└── README.md            # Project documentation
```

## Getting Started

To get started with this project, follow these steps:

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/marketing-landing-page.git
   cd marketing-landing-page
   ```

2. **Install dependencies:**

   If you have npm installed, run the following command to install any necessary dependencies:

   ```bash
   npm install
   ```

3. **Open the landing page:**

   You can open the `src/index.html` file in your web browser to view the landing page.

## Features

- Responsive design that looks great on all devices.
- Interactive elements powered by JavaScript.
- Customizable styles to match your branding.

## Contributing

If you would like to contribute to this project, please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.# douglas-landing



<!-- Fullscreen Blocker Overlay -->
        <div id="audio-warning-blocker" class="fixed inset-0 z-50 flex items-center justify-center bg-black/90">
            <div class="bg-red-900 text-white px-6 py-4 rounded-lg shadow-lg text-lg font-semibold flex items-center gap-2 flex-col md:flex-row">
                <div class="flex items-center gap-2 mb-4 md:mb-0">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M9 19V6l-2 2H5a2 2 0 00-2 2v4a2 2 0 002 2h2l2 2zm7-7a4 4 0 00-4-4m0 8a4 4 0 004-4m0 0V7m0 5v5"></path>
                    </svg>
                    Ative o áudio para uma melhor experiência!
                </div>
                <button id="close-audio-warning-blocker" class="bg-darkblue text-gold px-3 py-1 rounded hover:bg-goldDark hover:text-white transition">OK</button>
            </div>
        </div>
        <script>
            document.addEventListener('DOMContentLoaded', function () {
                const blocker = document.getElementById('audio-warning-blocker');
                const closeBtn = document.getElementById('close-audio-warning-blocker');
                closeBtn.addEventListener('click', function () {
                    blocker.style.display = 'none';
                });
                // Prevent scrolling while blocker is visible
                document.body.style.overflow = 'hidden';
                closeBtn.addEventListener('click', function () {
                    document.body.style.overflow = '';
                });
            });
        </script>