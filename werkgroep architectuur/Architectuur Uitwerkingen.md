# Archimate tekening
## Archimate 3.2 raw file
(Generieke Functie Toestemmingen.xml) apart in deze repo voor gebruik in Archimate3.2 ondersteunende tools zoals Archi

## Archimate 3.2 PNG
![Default View](https://github.com/minvws/generiekefuncties-toestemming/assets/123090714/d9706de6-eba3-4ace-b911-d2ac602b94b2)


# Sequentiediagrammen
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
## Sequentiediagram 2: Zorgaanbieder gebruikt PDP s2 <-> TV synced als PDP
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
    PAP s1 ->> PDP s2: sync & provide national policies (foreach BSN Data-aanbod)
    ZV ->> XIS: Fetch patientdata [BSN]
    XIS ->> XIS data-aanbieder: Query [BSN]
    XIS data-aanbieder ->> PEP s2: Query [BSN] allowed?
    PEP s2 ->> PDP s2: check local consent[BSN]
    PDP s2 ->> PEP s2: deny
    PEP s2 ->> PDP s2: check national consent [BSN]
    PDP s2 ->> PEP s2: permit [BSN]
    PEP s2 ->> XIS data-aanbieder: permit [BSN]
    XIS data-aanbieder ->> XIS: data [BSN]
```


