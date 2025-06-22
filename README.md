# Minecraft Mod Updater & Builder

<!--
TODO: Replace these badge URLs with your own once the repo is public.
You can generate them at https://shields.io/
-->
![License](https://img.shields.io/github/license/BryantWelch/mcmodupdate.app?style=for-the-badge)
![Issues](https://img.shields.io/github/issues/BryantWelch/mcmodupdate.app?style=for-the-badge)
![Forks](https://img.shields.io/github/forks/BryantWelch/mcmodupdate.app?style=for-the-badge)
![Stars](https://img.shields.io/github/stars/BryantWelch/mcmodupdate.app?style=for-the-badge)

A powerful web-based tool to update your Minecraft mods, discover new ones, and build modpacks with ease, all using the official Modrinth API.

### **[Live Site: mcmodupdate.app](https://mcmodupdate.app/)**

---

![Recording 2025-06-22 at 02 06 36](https://github.com/user-attachments/assets/aeb3e94e-068e-4fa4-a960-1b221ab5bc9a)


## About The Project

This tool was built to solve two common problems for Minecraft players: the tedious process of manually updating dozens of mods, and the challenge of building a new mod list with all the correct dependencies.

MC Updater provides a simple, elegant solution by allowing you to either drag-and-drop your existing `.jar` files or search for new mods directly. It then uses a powerful, hash-based search to accurately identify your mods on Modrinth and find the latest compatible versions for your chosen Minecraft version and mod loader.

## Key Features

*   **Accurate Mod Identification:** Uses a **hash-first search** for 100% accuracy, with a smart ID/Name search as a fallback.
*   **Automatic Dependency Resolution:** Automatically finds and includes required dependencies (like APIs and libraries) for your mods.
*   **Mod Discovery:** A built-in search bar allows you to find and add new mods directly from the Modrinth database.
*   **Rich Results:** View detailed information for each mod, including its icon, author, description, download count, and changelog.
*   **Modpack Export:** Download your entire updated mod list as a standard `.mrpack` file, ready to be imported into launchers like the Modrinth App, Prism, or ATLauncher.
*   **Intelligent API Handling:** Automatically handles Modrinth API rate limits with a transparent pausing and resuming process.
*   **Modern UI:** A clean, responsive, and user-friendly interface with helpful features like custom alerts and scroll-to-top/bottom buttons.

## How To Use

1.  **Select Your Target:** Choose your desired mod loader (Fabric, Forge, etc.) and Minecraft version from the dropdown menus.
2.  **Add Your Mods:**
    *   **To Update:** Drag and drop your existing `.jar` files into the upload area.
    *   **To Discover:** Use the search bar to find and add new mods from Modrinth.
3.  **Process Your List:** Click the "Update" button.
4.  **Review & Download:** The tool will find the latest compatible versions and all required dependencies. You can then download the files individually or as a complete `.mrpack`.

## Tech Stack

This project was built with a focus on performance and accessibility, using modern web standards without a heavy framework.

*   Vanilla HTML, CSS, and JavaScript
*   [JSZip](https://stuk.github.io/jszip/) - For reading `.jar` file contents in the browser.
*   [TOML](https://github.com/BinaryMuse/toml-node) - For parsing `mods.toml` files.
*   [Marked.js](https://marked.js.org/) - For rendering changelogs from Markdown.
*   [CryptoJS](https://github.com/brix/crypto-js) - For calculating SHA-1 file hashes.
*   [Modrinth API](https://docs.modrinth.com/) - For all mod and version data.

## Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Acknowledgments

*   A huge thank you to the **Modrinth Team** for providing a free, powerful, and well-documented API that makes tools like this possible.
