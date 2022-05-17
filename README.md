# [GMHI Webtool](https://danielchang2002.github.io/GMHI) 💩

[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![D3][d3]][d3-url]

## Description

An [interactive web-app](https://danielchang2002.github.io/GMHI) that analyzes MetaPhlAn outputs ran on gut microbiome samples.

## Usage

1. Run [MetaPhlAn](https://github.com/biobakery/MetaPhlAn) on your fastq file(s)

```bash
metaphlan metagenome_1.fastq --input_type fastq -o profiled_metagenome_1.txt
metaphlan metagenome_2.fastq --input_type fastq -o profiled_metagenome_2.txt
...
metaphlan metagenome_n.fastq --input_type fastq -o profiled_metagenome_n.txt
```

2. Merge outputs (if multiple) into a single file

```bash
merge_metaphlan_tables.py profiled_metagenome*.txt > merged_abundance_table.txt
```

3. Upload (merged) MetaPhlAn output to [GMHI webtool](https://danielchang2002.github.io/GMHI/)

4. Click display and look at the plots
![](images/1.png | width=100)
![](images/2.png | width=100)
![](images/3.png | width=100)
![](images/4.png | width=100)
![](images/5.png | width=100)

5. Export index information

<!-- MARKDOWN LINKS & IMAGES -->
[forks-shield]: https://img.shields.io/github/forks/danielchang2002/GMHI.svg?style=for-the-badge
[forks-url]: https://github.com/danielchang2002/GMHI/network/members
[stars-shield]: https://img.shields.io/github/stars/danielchang2002/GMHI.svg?style=for-the-badge
[stars-url]: https://github.com/danielchang2002/GMHI/stargazers
[issues-shield]: https://img.shields.io/github/issues/danielchang2002/GMHI.svg?style=for-the-badge
[issues-url]: https://github.com/danielchang2002/GMHI/issues
[license-shield]: https://img.shields.io/github/license/danielchang2002/GMHI.svg?style=for-the-badge
[license-url]: https://github.com/danielchang2002/GMHI/blob/main/LICENSE
[d3]: https://img.shields.io/badge/d3.js-F9A03C?style=for-the-badge&logo=d3.js&logoColor=white
[d3-url]: https://d3js.org/
[upload-box]: images/upload.png
