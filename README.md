Assignment_02_Genome_Exploration

Genome Exploration & Assembly Analysis of _Canis lupus_ using Galaxy.

# Genome Exploration of _Canis lupus_
_Species and Genome Information_

Species: _Canis lupus_

NCBI Assembly accession: GCA_905319855.2

Assembly level: Chromosome

Genome source: NCBI

FASTA filename: Canis_lupus.fasta

Approximate file size: 2.45 GB

# Objective

The objective of this activity was to explore the Canis lupus genome assembly using Galaxy. The activity focused on examining basic assembly statistics, sequence lengths, the effect of filtering short sequences, and the presence of possible open reading frames (ORFs).

# Tools Used

### **Part 2:** Fasta Statistics

The tool was used to obtain the total assembly length, number of sequences, minimum and maximum sequence length, mean sequence length, N50, L50, and GC content.

<img width="1818" height="1014" alt="image" src="https://github.com/user-attachments/assets/44f782c7-d884-46ef-906d-74a9d6d2fbb6" />
Figure 2. Assembly Statistics of the _Canis lupus_ genome generated using Fasta Statistics tool.

### **Part 3:** Compute sequence length

This tool was used to determine the length of each FASTA sequence. The five longest sequences were identified and recorded.

<img width="1742" height="1072" alt="image" src="https://github.com/user-attachments/assets/715aa596-40ba-41ba-a71b-823f1cfd4edd" />
Figure 3. Results of the Compute Sequence Length tool showing the lengths of the Canis lupus genome sequences.

### **Part 4:** Filter sequences by length & Fasta Statistics

A copy of the original genome was filtered using a minimum sequence length of 10,000 bp (10 kb). Fasta Statistics was then used again to compare the original and filtered genome.

<img width="1743" height="1072" alt="image" src="https://github.com/user-attachments/assets/d496bd42-1078-409e-8c85-418a67689f89" />
Figure 4. Result of the Filter Sequences by Length tool applied to the Canis lupus genome assembly in Galaxy. The resulting FASTA dataset contains 82 sequences.

### **Part 5:** Filter FASTA & getorf

The **Filter FASTA** tool was first used to select the sequence CAJNRB020000009.1 from the genome. The selected sequence was then analyzed using the **getorf** tool. The minimum nucleotide size of an ORF was set to 300 bp, and ORFs in the reverse complement were also included. The analysis produced 206 ORFs, with the longest ORF being 3,441 bp (CAJNRB020000009.1_15). Several ORF entries were inspected. The results demonstrate that a genome can contain sequences that could potentially code for proteins, but an ORF is not automatically a real gene and requires additional evidence for confirmation.

<img width="1746" height="1073" alt="image" src="https://github.com/user-attachments/assets/63972c31-c97b-4cab-b2bd-be7f4fb9cf96" />
Figure 5. Result of the Filter FASTA tool used to select the Canis lupus sequence CAJNRB020000009.1 for ORF analysis. One sequence was retained while 81 sequences were discarded.

<img width="1744" height="1071" alt="image" src="https://github.com/user-attachments/assets/6b21812e-76ed-482b-987a-c2f7e7c5bd61" />
Figure 6. Output of the getorf tool showing predicted open reading frames (ORFs) from the selected Canis lupus sequence. A total of 206 ORFs were identified, with the longest ORF (CAJNRB020000009.1_15) having a length of 3,441 bp.

## Important Results

The genome had a total assembly length of approximately 2.45 Gb. The scaffold N50 was 65,778,685 bp, with an L50 of 15, while the longest scaffold was approximately 124,665,963 bp and a minimum sequence length of 16,690 bp. The GC content was 41.49%.

Filtering sequences below 10 kb did not change the main assembly statistics because the shortest sequence in the original assembly was already 16,690 bp. Therefore, there were no sequences below the 10-kb filtering cutoff.

The ORF analysis found 206 ORFs, with the longest being 3,441 bp. This demonstrated that genome sequences can contain regions that could potentially code for proteins, but an ORF is not automatically a real gene as it requires additional evidence for confirmation.

## Short Interpretation

The results suggest that the Canis lupus genome assembly contains many long sequences, including very long scaffolds. The N50 and L50 values indicate that a large part of the genome is contained in a relatively small number of long scaffolds. The filtering experiment showed that sequences shorter than 10 kb were not present in the assembly, so removing them did not affect the main statistics. The ORF analysis showed that the genome contains regions that may potentially code for proteins, but these regions cannot automatically be considered real genes without additional evidence.

## Galaxy History

A screenshot of the Galaxy History showing the analysis steps.

<img width="1276" height="674" alt="image" src="https://github.com/user-attachments/assets/14d4e4fa-7e10-4f82-bc6e-a4f547036d8d" />
Figure 7. Galaxy history showing the tools and datasets used for this genome analysis activity. 
