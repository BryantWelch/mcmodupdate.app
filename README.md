# Minecraft Mod Updater & Builder

A powerful web-based tool to update Minecraft mods, discover new content, and build modpacks with ease using the official Modrinth API.

### **[🚀 Live Site: mcmodupdate.app](https://mcmodupdate.app/)**

---

![Minecraft Mod Updater Demo](https://github.com/user-attachments/assets/32c54e61-990e-486a-8ea4-63364ff43911)



## 🎯 About The Project

This tool was built to solve two common problems for Minecraft players: the tedious process of manually updating large collections, and the challenge of building a new list with all required dependencies.

Minecraft Mod Updater lets you drag-and-drop existing `.jar`, `.zip`, and `.mrpack` files, or search Modrinth directly for new content. It uses a hash-first identification pipeline to find accurate matches and resolve compatible versions for your selected Minecraft version and loader.

## ✨ Key Features

### Core Functionality
*   **Accurate Mod Identification:** Uses a **hash-first search** for 100% accuracy, with smart ID/Name search as fallback
*   **Recursive Dependency Resolution:** Automatically finds and includes required dependencies, including dependency chains
*   **Conflict Detection:** Flags incompatible dependency declarations and shows detailed conflict breakdowns
*   **Mod Discovery:** Built-in search to find and add content directly from Modrinth's database
*   **Modpack Export:** Download as standard `.mrpack` files for easy import into launchers

### Platform Support
*   **Fabric** - Full support with latest versions
*   **Forge** - Complete compatibility 
*   **NeoForge** - Modern Forge alternative support
*   **Quilt** - Fabric fork compatibility
*   **All Minecraft Versions** - From legacy to latest releases

### Supported Content Types
*   **Mods** (`.jar`, `.zip`)
*   **Resource Packs** (`.zip`)
*   **Shader Packs** (`.zip`)
*   **Data Packs** (`.zip`)
*   **Plugins** (`.jar`)
*   **Modpacks** (`.mrpack`)

### Performance & UX
*   **Smart Caching** - Session-based caching reduces API calls and improves speed
*   **Batch Processing** - Efficient handling of large mod collections
*   **Rate Limit Handling** - Transparent API rate limit management with countdown
*   **Bulk Actions** - Select multiple results for faster download workflows
*   **Mobile Responsive** - Works perfectly on phones and tablets
*   **Modern UI** - Clean, dark theme with intuitive controls

### Rich Information Display
*   **Mod Icons & Details** - Visual mod information with descriptions
*   **Author Information** - Direct links to mod creators
*   **Download Statistics** - See mod popularity metrics  
*   **Changelogs** - View what's new in mod updates
*   **Categories & Tags** - Understand content types at a glance
*   **Dependency & Conflict Indicators** - See why a dependency was added and where incompatibilities exist

### Result States
*   **Green:** Update found
*   **Blue:** Auto-added dependency
*   **White:** Already up to date
*   **Yellow:** No compatible version for selected target
*   **Red:** Not found or failed to process

## 🚀 How To Use

1.  **Select Your Target:** Choose your mod loader (Fabric, Forge, NeoForge, Quilt) and Minecraft version
2.  **Add Your Mods:**
    *   **To Update:** Drag and drop `.jar`, `.zip`, or `.mrpack` files into the upload area
    *   **To Discover:** Use the search bar to find mods, modpacks, shaders, resource packs, data packs, and plugins from Modrinth
3.  **Process Your List:** Click the "Update" button and watch the magic happen
4.  **Review & Download:** Inspect updates, dependencies, and conflicts, then download individually, in bulk, as a `.zip`, or as a complete `.mrpack`

## 🛠️ Tech Stack

Built with performance and accessibility in mind, using modern web standards without heavy frameworks.

### Frontend
*   **Vanilla HTML, CSS, and JavaScript** - No framework bloat, maximum performance
*   **Responsive Design** - Mobile-first approach with desktop enhancements
*   **Progressive Enhancement** - Core workflows remain straightforward across modern browsers and device sizes

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

## 📄 License

Distributed under the **Mozilla Public License 2.0**. See `LICENSE` for more information.

## 🙏 Acknowledgments

*   **[Modrinth Team](https://modrinth.com)** - For providing an amazing, free API that makes tools like this possible
*   **Minecraft Modding Community** - For creating the incredible mods that make Minecraft endlessly enjoyable
*   **Open Source Tools & Libraries** - The projects that power this app

---

**Made with ❤️ for the Minecraft community**
