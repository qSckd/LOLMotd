# LOLMotd - BungeeCord ONLY

## Description
Since "choice21" decided to leak a very old useless and ratted version of the plugin, i decided to open source this and improve the plugin to keep his version outdated and avoid people getting his rat.

LOLMotd is a lightweight and customizable BungeeCord plugin designed to provide dynamic "Message of the Day" (MotD) functionality for your Minecraft network. It allows server administrators to display different messages to players based on their client version, ensuring compatibility and an optimal experience for all users.

This plugin was made for my server (Imanity Network - imanity.lol) thats why the name is LOLMotd and then was given to RagePvP Network, which had 100 players running this plugin with no issues.
![img.png](img.png)

New servers using the plugin:

<img width="629" height="220" alt="image" src="https://github.com/user-attachments/assets/bad08b19-8f3e-4ff6-a18e-658460e7a494" />

If you use my plugin dm me on discord "matthew.tf" to get it up here!

For the gradient, you need to use the legacy format in order for it to work.

## Features
*   **Version-Specific MotDs:** Display distinct messages for modern (1.16+) and legacy Minecraft clients.
*   **Customizable Messages:** Easily configure your server's MotD with rich text formatting, color codes (`&`), and newline support (`%newline%`).
*   **On-the-Fly Reload:** Administrators can reload the plugin's configuration without restarting the BungeeCord proxy.
*   **Lightweight and Efficient:** Designed for minimal impact on proxy performance.

## Installation
To install the LOLMotd plugin on your BungeeCord proxy, follow these steps:

1.  **Download the Plugin:**
    *   Obtain the latest `LOLMotd-<version>.jar` file from the [releases page](https://github.com/qSckd/LOLMotd/releases) (link to be updated when releases are available).

2.  **Place in `plugins` folder:**
    *   Stop your BungeeCord proxy.
    *   Place the downloaded `LOLMotd-<version>.jar` file into your BungeeCord proxy's `plugins/` directory.

3.  **Start the Proxy:**
    *   Start your BungeeCord proxy. The plugin will automatically generate its configuration file (`config.yml`) in `plugins/LOLMotd/`.

## Configuration
After the first run, a `config.yml` file will be generated in `plugins/LOLMotd/`. You can edit this file to customize your Message of the Day for different client versions. 

**Example `config.yml`:**
```yaml
motds:
  # Modern MOTD for newer client versions. (1.16 to latest)
  # - "" is a new line that will be shown for the motd or you can use the following ▼▼
  #
  # IMPORTANT:
  # To use gradients you will need the legacy format.
  #
  # Use '&' for color codes and '%newline%' for an additional line break within a single list item.
  modern:
    - "      &4▪▪  &x&9&7&0&0&0&0&lI&x&9&1&0&0&0&0&lM&x&8&A&0&0&0&0&lA&x&8&4&0&0&0&0&lN&x&7&D&0&0&0&0&lI&x&7&7&0&0&0&0&lT&x&7&0&0&0&0&0&lY &x&9&7&9&7&9&7&lN&x&9&1&9&1&9&1&lE&x&8&A&8&A&8&A&lT&x&8&4&8&4&8&4&lW&x&7&D&7&D&7&D&lO&x&7&7&7&7&7&7&lR&x&7&0&7&0&7&0&lK &8▸ &7「 1.16 - 1.21x 」 &4▪▪ %newline%&8➥ &x&B&0&7&8&2&E&lN&x&B&D&8&B&3&5&lO&x&C&A&9&E&3&C&lV&x&D&8&B&1&4&3&lE&x&E&5&C&3&4&9&lD&x&F&2&D&6&5&0&lA&x&F&F&E&9&5&7&lD &8┃ &x&7&F&8&0&7&DA&x&8&7&8&8&8&5p&x&8&F&9&0&8&Do&x&9&7&9&8&9&5y&x&9&F&A&0&9&Ea&x&A&7&A&8&A&6n&x&A&F&B&0&A&Eo&x&B&7&B&8&B&6s &x&B&F&C&0&B&Ed&x&C&7&C&7&C&6o&x&C&F&C&F&C&En&x&D&7&D&7&D&6a&x&D&F&D&F&D&Fn&x&E&7&E&7&E&7d&x&E&F&E&F&E&Fo &x&F&7&F&7&F&7e&x&F&F&F&F&F&Fn &x&B&0&7&8&2&E&nt&x&B&5&7&F&3&0&ni&x&B&9&8&5&3&3&ne&x&B&E&8&C&3&5&nn&x&C&3&9&3&3&8&nd&x&C&7&9&9&3&A&na&x&C&C&A&0&3&C&n.&x&D&1&A&7&3&F&ni&x&D&5&A&D&4&1&nm&x&D&A&B&4&4&4&na&x&D&E&B&A&4&6&nn&x&E&3&C&1&4&9&ni&x&E&8&C&8&4&B&nt&x&E&C&C&E&4&D&ny&x&F&1&D&5&5&0&n.&x&F&6&D&C&5&2&nl&x&F&A&E&2&5&5&no&x&F&F&E&9&5&7&nl"
  # Legacy MOTD for older client versions. (1.15 to 1.0)
  # - "" is a new line that will be shown for the motd or you can use the following ▼▼
  # Use '&' for color codes and '%newline%' for an additional line break within a single list item.
  legacy:
    - "&4&lIMANITY &F&lNETWORK &7| &8「 1.16 - 1.21x 」"
    - "&fServidor solo disponible para 1.16 en adelante!"
```

*   `motds.modern`: This message will be displayed to players using Minecraft client versions 1.16 and above.
*   `motds.legacy`: This message will be displayed to players using older Minecraft client versions (before 1.16).

**Color Codes:** You can use the `&` symbol followed by a color code (e.g., `&a` for green) to format your messages. For a full list of color codes, refer to the [Minecraft Wiki](https://minecraft.fandom.com/wiki/Formatting_codes).

**Newlines:** Use `%newline%` in your configuration to create a new line in your MotD.

## Usage
Once the plugin is installed and configured, players connecting to your BungeeCord network will see the custom MotD based on their client version.

**Admin Commands:**
*   `/lolmotd reload`: Reloads the plugin's `config.yml` file. Requires the permission `lolmotd.reload`.

## Compiling from Source
If you wish to compile LOLMotd from its source code, follow these steps:

1.  **Prerequisites:**
    *   Java Development Kit (JDK) 8 or newer.
    *   Maven (for dependency management and building).

2.  **Clone the Repository:**
    ```bash
    git clone https://github.com/qSckd/LOLMotd.git
    cd LOLMotd
    ```

3.  **Compile the Plugin:**
    ```bash
    mvn clean package
    ```
    *   This will generate a `LOLMotd-<version>.jar` file in the `target/` directory. This is the file you would place in your BungeeCord proxy's `plugins/` folder.

## Contributing
We welcome contributions to LOLMotd! To contribute, please follow these steps:

1.  Fork the repository.
2.  Create a new branch (`git checkout -b feature/your-feature-name`).
3.  Make your changes and ensure your code adheres to BungeeCord plugin development best practices.
4.  Commit your changes (`git commit -m 'Add new feature'`).
5.  Push to the branch (`git push origin feature/your-feature-name`).
6.  Open a Pull Request.

Please ensure your code is well-documented and includes appropriate tests if applicable.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.





