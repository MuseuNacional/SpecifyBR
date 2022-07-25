# Modelo de Organização do Museu Nacional-UFRJ


```mermaid
flowchart TB
  subgraph Departamentos
      direction LR    
      subgraph Entomologia
      direction TB
        subgraph Entomologica
        direction TB
          c2(Blattodea)
          c3(Coleoptera)
          c4(Collembolla)
          c5(Diplura)
          c6(Diptera)
          c7(Ephemeroptera)
          c8(Hemiptera)
          c9(Hymenoptera)
          c10(Lepidoptera)
          c11(Mantodea)
          c12(Megaloptera)
          c13(Neuroptera)
          c14(Odonata)
          c15(Orthoptera)
          c16(Phasmatodea)
          c17(Plecoptera)
          c18(Protura)
          c19(Psocoptera)
          c20(Strepsiptera)
          c21(Trichoptera)
        end
      end
      subgraph Invertebrados
      direction TB
        c34(Celenterologia)
        c35(Crustacea)
        c36(Echinoderma)
        c37(Malacologia)    
        c38(Polychaeta)
        c39(Porifera)
        subgraph Aracnologia
        direction TB   
          c23(Aranea)
          c24(Aranea)
          c25(Opiliones)
          c26(Ordens Menores)
        end
        subgraph Invertebrados outros
        direction TB   
          c27(Ascidiacea)
          c28(Brachiopoda)
          c29(Bryozoa)
          c30(Mematoda)
          c31(Nemertea)
          c32(Platyelminthes)
          c33(Tardigrada)
        end
      end
  end
```
