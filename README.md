# AssetRegistry

**Official Asset Registry for Cryonic Engine**  
A central listing of assets for Cryonic Engine, providing easy access to assets compatible with the engine.

## Overview

The AssetRegistry acts as the main hub for locating, downloading, and managing assets specifically designed for Cryonic Engine. This repository includes a JSON file listing all supported assets, which the engine’s Asset Manager can access to automatically update and integrate assets.

## How It Works

The `assets.json` file in this repository contains a structured list of available assets. Each entry includes:
- **Name**: The name of the asset.
- **URL**: A link to the asset’s GitHub repository.
- **Category**: The category the asset belongs to. The Categories are General, Scripts, Textures, Models, Environments, Audio, GUI, Templates, and Tools.

By pulling data from this JSON file, Cryonic Engine can retrieve supported assets and be able to install them to projects.

## JSON Structure Example

```json
[
    {
        "name": "Example Asset",
        "url": "https://github.com/YourUsername/ExampleAsset",
        "category": "General"
    }
]
```

## Adding New Assets / Contributing
1. Create a GitHub repository for the new asset.<br/>
2. Add a manifest.json file and include all relevant asset information. You can refer to the [AI Pathfinding manifest file](https://github.com/CryonicEngine/AI-Pathfinding/blob/main/manifest.json) as an example.<br/>
3. Fork this GitHub repository.<br/>
4. Update assets.json to include the new asset at the bottom.<br/>
5. Submit a pull request.<br/>

## License
This registry is licensed under the [GPL-3.0 License](LICENSE). Refer to individual asset repositories for their respective licenses.
