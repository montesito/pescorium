# Orbiscator Biological Registry

This repository serves as the centralized source of truth for the biological data used in the **Orbiscator** application. 

By managing these resources here, we ensure that species information, translations, and illustrations can be updated independently of the application code.

## Structure

### 📂 Registry/
Contains the core data in JSON format.
- `species_registry.json`: The master list of all supported species.
  - Supports: Spanish (`es`), English (`en`), French (`fr`), and German (`de`).
  - Includes: ID, Scientific Name, Family, Localized Names, and Descriptions.

### 📂 Vault/
Contains the visual assets.
- High-fidelity `.png` illustrations for each species.
- **Naming Convention**: Filenames must match the `illustrationName` field in the JSON file (e.g., `species_brown_trout.png`).

## Contribution Workflow
To add or update a species:
1. Edit `Registry/species_registry.json`.
2. Upload the corresponding illustration to `Vault/` if applicable.
3. Commit and push changes.
