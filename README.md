
# **Wynncraft Territory Map -> JSON**

This repository exists to maintain a comprehensive and up-to-date replica of the **Wynncraft guild territory map**. The project will continue until such a time until the API adds these fields. My goal is to ensure that all data—such as resources, trade routes, and guild ownership—remains consistent with how it exists. I welcome any contributions.

---

## **Project Overview**

The `territories.json` file contains key details for each territory, including:

- **Resources**: Details available resources such as emeralds, ore, crops, fish, and wood
- **Trade Routes**: Lists trade connections between territories.
- **Location**: Specifies the geographical start and end points of each territory when available.
- **Guild**: This field is intentionally left as **blank strings** (`""`) due to the dynamic nature of guild ownership in Wynn.

It is important to note that some fields, such as **Location**, may be missing for certain territories due to **API Bugs**.

---

## **Contribution Guidelines**

I welcome contributions to this project via **pull requests**. Please follow the guidelines below when submitting updates:

### **Fields to Update**
- **Resources**: Ensure that resource data reflects the most current information from Wynncraft.
- **Trade Routes**: Add or update connections between territories based on the latest trade routes.
- **Guild Fields**: Although guild ownership frequently changes, you are encouraged to update these fields with the most current information.
- **Missing Fields**: Fill in missing data (e.g., Location) where possible, especially for fields not provided by the current API.

### **Steps to Contribute**
1. **Fork** the repository.
2. **Modify** the `territories.json` file while maintaining the data structure (outlined below).
3. **Submit** a pull request with a brief summary of the changes made.

The **expected data structure** is as follows:

\`\`\`json
{
  "territoryName": {
    "guild": {
      "uuid": "",
      "name": "",
      "prefix": ""
    },
    "acquired": "",
    "resources": {
      "emeralds": "number",
      "ore": "number",
      "crops": "number",
      "fish": "number",
      "wood": "number"
    },
    "trade_routes": [
      "Other Territory Name"
    ],
    "location": {
      "start": [x, y],
      "end": [x, y]
    }
  }
}
\`\`\`

---

## **Field Inconsistencies**

Due to limitations with the API, some territories may have missing fields such as **Location** or **Guild** data. If you have access to this information, I encourage you to provide updates. Guild fields are intentionally left as empty strings.

---

### **Project Lifespan**

This project will remain active until the Wynncraft Guild Territory API adds the missing fields present in the JSON. 
