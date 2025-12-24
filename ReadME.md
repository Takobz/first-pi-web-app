# First Pi Web App

## High Level Architecture

This project attempts to achieve the set up discribe below by the mermaid chart.  

```mermaid
flowchart LR
    A[Internet] -- HTTPS Traffic --> B[Nginx <br/> Container]

    subgraph Docker Network
        B -- Route Calls --> C[Web App]
        B -- Route Calls --> D[Web App 2]
    end

    C <-.-> E[External <br/> Serivces]
    D <-.-> E
```

If the above chart doesn't render use: [mermaid editor](https://mermaid.live/) to view.

## Set Up Explained
