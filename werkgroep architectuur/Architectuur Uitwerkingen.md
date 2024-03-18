# Archimate 3.2 SVG (afdruk van de raw file hieronder)

# Archimate 3.2 XML (Archimate Export Format(raw))
## deze file kan ingelezen worden in tools (zoals open source Archi) die de archimate 3.2 modeleertaal ondersteunen
## raw file


# Sequentiediagrammen (MerMaid)
## Sequentiediagram 1: Zorgaanbieder gebruikt TV als PDP
```mermaid
sequenceDiagram
    Title Zorgaanbieder gebruikt TV als PDP
    autonumber
    box datavraag
    actor ZV
    participant XIS
    end
    box Data-aanbod
    participant XIS data-aanbieder
    participant PEP s2
    participant PDP s2
    participant PAP s2
    end
    box GF toestemming
    actor admin
    participant PDP s1
    participant PAP s1
    end
    PAP s2 ->> PDP s2: manage & provide local policies
    PAP s1 ->> PDP s1: manage & provide national policies
    ZV ->> XIS: Fetch patientdata [BSN]
    XIS ->> XIS data-aanbieder: Query [BSN]
    XIS data-aanbieder ->> PEP s2: Query [BSN] allowed?
    PEP s2 ->> PDP s2: check local consent[BSN]
    PDP s2 ->> PEP s2: deny
    PEP s2 ->> PDP s1: check national consent [BSN]
    PDP s1 ->> PAP s1: retrieve policies
    PAP s1 ->> PDP s1: return policies
    PDP s1 ->> PEP s2: permit [BSN]
    PEP s2 ->> XIS data-aanbieder: permit [BSN]
    XIS data-aanbieder ->> XIS: data [BSN]
```
## Sequentiediagram 2
