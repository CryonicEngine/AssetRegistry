# AssetRegistry

**Official Asset Registry for [Your Engine Name]**  
A central listing of assets for [Your Engine Name], providing easy access to resources, tools, and updates compatible with the engine.

## Overview

The AssetRegistry acts as the main hub for locating, downloading, and managing assets specifically designed for [Your Engine Name]. This repository includes a JSON file listing all available assets, which the engine’s Asset Manager can access to automatically update and integrate new resources.

## How It Works

The `asset_registry.json` file in this repository contains a structured list of available assets. Each entry includes:
- **Name**: The name of the asset.
- **Repository URL**: A link to the asset’s GitHub repository.
- **Manifest URL**: A link to a detailed JSON file (in each asset’s repository) that contains additional metadata like version, supported engine versions, dependencies, etc.

By pulling data from this central JSON file, [Your Engine Name] can retrieve the latest versions and descriptions of available assets seamlessly.

## JSON Structure Example

```json
[
    {
        "name": "Basic Texture Pack",
        "url": "https://github.com/YourUsername/BasicTexturePack",
        "category": "Scripts"
    }
]

Each entry provides a direct link to the asset’s repository and the specific manifest file, making it easy for the engine to fetch detailed information.

## Adding New Assets
Create a GitHub repository for the new asset.
Add a asset_manifest.json file in the asset repository containing information such as version, description, supported versions, etc.
Update asset_registry.json in this repository to include the new asset with its name, repository URL, and manifest URL.
Submit a pull request if you’re a contributor, or contact the repository owner for inclusion.

## License
This registry is licensed under the [GPL-3.0 License](LICENSE). Refer to individual asset repositories for their respective licenses.

## Contributing
We welcome contributions! If you’d like to add an asset to the registry or update an existing one, please follow the steps under “Adding New Assets” and submit a pull request. For major updates or questions, please open an issue.
