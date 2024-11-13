# AssetRegistry

**Official Asset Registry for Cryonic Engine**  
A central listing of assets for Cryonic Engine, providing easy access to resources, tools, and updates compatible with the engine.

## Overview

The AssetRegistry acts as the main hub for locating, downloading, and managing assets specifically designed for Cryonic Engine. This repository includes a JSON file listing all available assets, which the engine’s Asset Manager can access to automatically update and integrate new resources.

## How It Works

The `assets.json` file in this repository contains a structured list of available assets. Each entry includes:
- **Name**: The name of the asset.
- **URL**: A link to the asset’s GitHub repository.
- **Category**: The category the asset belongs to. Current categories are General, Scripts, Textures, Models, Environments, Audio, GUI, Templates, and Tools.

By pulling data from this JSON file, Cryonic Engine can retrieve supported assets and be able to install them to projects.

## JSON Structure Example

```json
[
    {
        "name": "Basic Asset",
        "url": "https://github.com/YourUsername/ExampleAsset",
        "category": "General"
    }
]
```

## Adding New Assets
Create a GitHub repository for the new asset.<br/>
Add a asset_manifest.json file in the asset repository containing information such as version, description, supported versions, etc.
Update asset_registry.json in this repository to include the new asset with its name, repository URL, and manifest URL.
Submit a pull request if you’re a contributor, or contact the repository owner for inclusion.

## License
This registry is licensed under the [GPL-3.0 License](LICENSE). Refer to individual asset repositories for their respective licenses.

## Contributing
We welcome contributions! If you’d like to add an asset to the registry or update an existing one, please follow the steps under “Adding New Assets” and submit a pull request. For major updates or questions, please open an issue.
