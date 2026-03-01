# Minecraft Mod Updater & Builder

A powerful web-based tool to update your Minecraft mods, discover new ones, and build modpacks with ease, all using the official Modrinth API.

### **[🚀 Live Site: mcmodupdate.app](https://mcmodupdate.app/)**

---

![MC Mod Updater Demo](https://github.com/user-attachments/assets/32c54e61-990e-486a-8ea4-63364ff43911)



## 🎯 About The Project

This tool was built to solve two common problems for Minecraft players: the tedious process of manually updating dozens of mods, and the challenge of building a new mod list with all the correct dependencies.

MC Mod Updater provides a simple, elegant solution by allowing you to either drag-and-drop your existing `.jar` files, your current `.mrpack`, or search for new mods directly. It then uses a powerful, hash-based search to accurately identify your mods on Modrinth and find the latest compatible versions for your chosen Minecraft version and mod loader.

## ✨ Key Features

### Core Functionality
*   **Accurate Mod Identification:** Uses a **hash-first search** for 100% accuracy, with smart ID/Name search as fallback
*   **Automatic Dependency Resolution:** Automatically finds and includes required dependencies (APIs, libraries, etc.)
*   **Mod Discovery:** Built-in search to find and add new mods directly from Modrinth's database
*   **Modpack Export:** Download as standard `.mrpack` files for easy import into launchers

### Platform Support
*   **Fabric** - Full support with latest versions
*   **Forge** - Complete compatibility 
*   **NeoForge** - Modern Forge alternative support
*   **Quilt** - Fabric fork compatibility
*   **All Minecraft Versions** - From legacy to latest releases

### Performance & UX
*   **Smart Caching** - Session-based caching reduces API calls and improves speed
*   **Batch Processing** - Efficient handling of large mod collections
*   **Rate Limit Handling** - Transparent API rate limit management with countdown
*   **Mobile Responsive** - Works perfectly on phones and tablets
*   **Modern UI** - Clean, dark theme with intuitive controls

### Rich Information Display
*   **Mod Icons & Details** - Visual mod information with descriptions
*   **Author Information** - Direct links to mod creators
*   **Download Statistics** - See mod popularity metrics  
*   **Changelogs** - View what's new in mod updates
*   **Categories & Tags** - Understand mod types at a glance

## 🚀 How To Use

1.  **Select Your Target:** Choose your mod loader (Fabric, Forge, NeoForge, Quilt) and Minecraft version
2.  **Add Your Mods:**
    *   **To Update:** Drag and drop existing `.jar` files or your `.mrpack` into the upload area
    *   **To Discover:** Use the search bar to find new mods from Modrinth
3.  **Process Your List:** Click the "Update" button and watch the magic happen
4.  **Review & Download:** Get latest compatible versions plus dependencies that you can download individually, as a `.zip`, or as a complete `.mrpack`

## 🛠️ Tech Stack

Built with performance and accessibility in mind, using modern web standards without heavy frameworks.

### Frontend
*   **Vanilla HTML, CSS, and JavaScript** - No framework bloat, maximum performance
*   **Responsive Design** - Mobile-first approach with desktop enhancements
*   **Progressive Enhancement** - Works with JavaScript disabled (basic functionality)

### Libraries & APIs
*   **[JSZip](https://stuk.github.io/jszip/)** - Client-side `.jar` file reading and `.mrpack` creation
*   **[TOML.js](https://github.com/BinaryMuse/toml-node)** - Parse `mods.toml` files for mod identification
*   **[Marked.js](https://marked.js.org/)** - Render mod changelogs from Markdown
*   **[CryptoJS](https://github.com/brix/crypto-js)** - Calculate SHA-1 file hashes for accurate identification
*   **[Modrinth API](https://docs.modrinth.com/)** - All mod data, versions, and metadata

### Infrastructure
*   **[Netlify](https://netlify.com)** - Hosting with automatic deployments
*   **Custom Domain** - Professional presence at https://mcmodupdate.app

## 📊 Performance Features

*   **Session Caching** - Reduces API calls by 60-80% on repeat operations
*   **Batch Processing** - Handle 100+ mods efficiently
*   **Smart Rate Limiting** - Automatic backoff with user-friendly countdown
*   **Optimized Assets** - Fast loading with proper caching headers
*   **Mobile Optimized** - Lightweight and fast on mobile devices

## 🤝 Contributing

Contributions make the open-source community amazing! Any contributions are **greatly appreciated**.

### Ways to Contribute
*   🐛 **Bug Reports** - Found an issue? Open an issue with details
*   💡 **Feature Requests** - Have an idea? Tag it with "enhancement" 
*   🔧 **Code Contributions** - Fork, branch, code, and PR!
*   📖 **Documentation** - Help improve guides and explanations
*   🌐 **Translations** - Help make it accessible worldwide

### Development Process
1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

## 📄 License

Distributed under the **Mozilla Public License 2.0**. See `LICENSE` for more information.

## 🙏 Acknowledgments

*   **[Modrinth Team](https://modrinth.com)** - For providing an amazing, free API that makes tools like this possible
*   **Minecraft Modding Community** - For creating the incredible mods that make Minecraft endlessly enjoyable
*   **Open Source Contributors** - Everyone who helps improve this tool

---

**Made with ❤️ for the Minecraft community**
