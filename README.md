Multi-CSAR datasets
===================
Supporting datasets for Multi-CSAR <https://github.com/ablab-nthu/Multi-CSAR>

Content
-------

Directory `inputs`:
```
.
├── BCEN                         // B. cenocepacia j2315
│   ├── Burkholderia_target.fna  // File of target draft genome for B. cenocepacia j2315
│   └── reference_genomes/       // Directory containing reference genomes
├── ECOL                         // E. coli K12
│   ├── E.Coli_target.fna        // File of target draft genome for E. Coli K12
│   └── reference_genomes/       // Directory containing reference genomes
├── MTUB                         // M. tuberculosis
│   ├── Mtub_target.fna          // File of target draft genome for M. tuberculosis
│   └── reference_genomes/       // Directory containing reference genomes
├── RSPH                         // R. sphaeroides 2.4.1
│   ├── Rhodobacter_target.fna   // File of target draft genome for R. sphaeroides 2.4.1
│   └── reference_genomes/       // Directory containing reference genomes
└── SAUR                         // S. aureus
    ├── Saureus_target.fna       // File of target draft genome for S. aureus
    └── reference_genomes/       // Directory containing reference genomes

```

Directory `outputs`:
```
.
├── BCEN                               // B. cenocepacia j2315
│   ├── multi-csar_nucmer              // Output of Multi-CSAR using NUCmer
│   │   ├── multi-csar.nuc.out         // File of scaffolds
│   │   └── multi-csar.nuc.out.fna     // File of scaffold sequences
│   ├── multi-csar_nucmer_WS           // Output of Multi-CSAR using NUCmer with weighting scheme
│   │   ├── multi-csar.nuc.ws.out      // File of scaffolds 
│   │   └── multi-csar.nuc.ws.out.fna  // File of scaffold sequences
│   ├── multi-csar_promer              // Output of Multi-CSAR using PROmer
│   │   ├── multi-csar.pro.out         // File of scaffolds 
│   │   └── multi-csar.pro.out.fna     // File of scaffold sequences
│   └── multi-csar_promer_WS           // Output of Multi-CSAR using PROmer with weighting scheme
│       ├── multi-csar.pro.ws.out      // File of scaffolds
│       └── multi-csar.pro.ws.out.fna  // File of scaffold sequences
├── ECOL                               // E. coli K12
│   ├── ...
│   .  
│   └── ...
├── MTUB/                              // M. tuberculosis
├── RSPH/                              // R. sphaeroides 2.4.1
└── SAUR/                              // S. aureus

```

Usage
-----
Download the zip file and upzip it on your system.

Under the multi-csar_datasets directory, one can use a dataset (e.g., BCEN) to run Multi-CSAR by using the following commend:

	multi-csar.php -t inputs/BCEN/Burkholderia_target.fna -r inputs/BCEN/reference_genomes/ --nuc -o example_out

