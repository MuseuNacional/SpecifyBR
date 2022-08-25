# Modelo de Organização do Museu Nacional-UFRJ

```mermaid
flowchart TB
  subgraph Departamentos
      direction TB    
      subgraph Entomologia
      direction LR
        subgraph Entomologica
        direction LR
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
      direction LR
        c34(Celenterologia)
        c35(Crustacea)
        click c35 href "https://github.com/edalcin/SpecifyBR/blob/main/organizacaoInstitucional/museuNacional/colecoes/crustaceae.md"
        c36(Echinoderma)
        click c36 href "https://github.com/edalcin/SpecifyBR/blob/main/organizacaoInstitucional/museuNacional/colecoes/echinoderma.md"
        c37(Mollusca)
        click c37 href "https://github.com/edalcin/SpecifyBR/blob/main/organizacaoInstitucional/museuNacional/colecoes/mollusca.md"
        c38(Polychaeta)
        click c38 href "https://github.com/edalcin/SpecifyBR/blob/main/organizacaoInstitucional/museuNacional/colecoes/polychaeta.md"
        c39(Porifera)
        click c39 href "https://github.com/edalcin/SpecifyBR/blob/main/organizacaoInstitucional/museuNacional/colecoes/porifera.md"
        subgraph Aracnologia
        direction LR   
          c23(Aranea)
          c24(Myriapoda)
          c25(Opiliones)
          c26(Ordens Menores)
        end
        subgraph Invertebrados outros
        direction LR   
          c27(Ascidiacea)
          c28(Brachiopoda)
          c29(Bryozoa)
          c30(Mematoda)
          c31(Nemertea)
          c32(Platyelminthes)
          c33(Tardigrada)
        end
      end
      subgraph Vertebrados
      direction LR   
        c40(Anfíbios)
        click c40 href "https://github.com/edalcin/SpecifyBR/blob/main/organizacaoInstitucional/museuNacional/colecoes/anfibios.md"
        c41(Ictiologia)
        click c41 href "https://github.com/edalcin/SpecifyBR/blob/main/organizacaoInstitucional/museuNacional/colecoes/ictiologia.md"
        c42(Mamíferos)
        c43(Ornitologia)
        click c43 href "https://github.com/edalcin/SpecifyBR/blob/main/organizacaoInstitucional/museuNacional/colecoes/ornitologia.md"
        c44(Répteis)
        click c44 href "https://github.com/edalcin/SpecifyBR/blob/main/organizacaoInstitucional/museuNacional/colecoes/repteis.md"
      end
end
```
