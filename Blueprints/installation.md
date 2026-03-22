
# Home Assistant Blueprint Installation Guide

This guide explains how to install and use blueprints in Home Assistant.

---

## Requirements

- Home Assistant is installed and running
- Access to **Settings → Automations & Scenes**

---

## Method 1 – Import via URL

1. Go to:
```
Settings → Automations & Scenes → Blueprints
```
2. Click:
```
Import Blueprint
```
3. Paste the blueprint URL (for example a GitHub link)
4. Click:
```
Preview → Import
```
5. The blueprint is now available
<br>

---

## Method 2 – Manual Installation

1. Go to your Home Assistant configuration folder:
```
/config/blueprints/automation/
```
2. Create a new file:
```
your_blueprint_name.yaml
```
3. Paste the blueprint YAML into the file
4. Save the file
5. Reload automations:
```
Settings → Developer Tools → YAML → Reload Automations
```
or restart Home Assistant
<br>

---

## Creating an Automation from a Blueprint
1. Go to:
```
Settings → Automations & Scenes
```
2. Click:
```
* Create Automation
```
3. Select:
```
From Blueprint
```
4. Choose your blueprint
5. Fill in the required inputs
6. Click:
```
Save
```
<br>

---

## Updating a Blueprint
1. Edit the blueprint YAML file
2. Reload automations or restart Home Assistant
⚠️ Note:
Changes apply to all automations using this blueprint

---

## Troubleshooting
### Blueprint not visible
- Reload automations
- Check YAML syntax

### Automation not working
- Verify inputs (entities, thresholds, time)
- Check logs:
```
Settings → System → Logs
```

### YAML errors
- Check indentation
- Use Developer Tools → YAML
```
