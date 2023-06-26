# Comparing `tmp/biopipen-0.8.0.tar.gz` & `tmp/biopipen-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biopipen-0.8.0.tar", max compression
+gzip compressed data, was "biopipen-0.9.0.tar", max compression
```

## Comparing `biopipen-0.8.0.tar` & `biopipen-0.9.0.tar`

### file list

```diff
@@ -1,161 +1,161 @@
--rw-r--r--   0        0        0       23 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/core/__init__.py
--rw-r--r--   0        0        0     1069 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/core/config.py
--rw-r--r--   0        0        0     1598 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/core/config.toml
--rw-r--r--   0        0        0      344 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/core/defaults.py
--rw-r--r--   0        0        0     2360 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/core/filters.py
--rw-r--r--   0        0        0      498 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/core/proc.py
--rw-r--r--   0        0        0     1586 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/core/testing.py
--rw-r--r--   0        0        0        0 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/ns/__init__.py
--rw-r--r--   0        0        0     6484 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/ns/bam.py
--rw-r--r--   0        0        0     3467 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/ns/bcftools.py
--rw-r--r--   0        0        0     5231 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/ns/bed.py
--rw-r--r--   0        0        0     2901 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/ns/cnv.py
--rw-r--r--   0        0        0    28348 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/ns/cnvkit.py
--rw-r--r--   0        0        0    26835 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/ns/cnvkit_pipeline.py
--rw-r--r--   0        0        0      484 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/ns/csv.py
--rw-r--r--   0        0        0     2228 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/ns/gene.py
--rw-r--r--   0        0        0     7423 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/ns/gsea.py
--rw-r--r--   0        0        0     3015 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/ns/misc.py
--rw-r--r--   0        0        0     4026 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/ns/plot.py
--rw-r--r--   0        0        0      565 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/ns/rnaseq.py
--rw-r--r--   0        0        0    28935 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/ns/scrna.py
--rw-r--r--   0        0        0    15622 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/ns/scrna_metabolic_landscape.py
--rw-r--r--   0        0        0     1455 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/ns/tcgamaf.py
--rw-r--r--   0        0        0    23074 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/ns/tcr.py
--rw-r--r--   0        0        0    15314 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/ns/vcf.py
--rw-r--r--   0        0        0     2224 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/ns/web.py
--rw-r--r--   0        0        0      212 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/reports/bam/CNAClinic.svelte
--rw-r--r--   0        0        0     1363 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/reports/bam/CNVpytor.svelte
--rw-r--r--   0        0        0      836 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/reports/bam/ControlFREEC.svelte
--rw-r--r--   0        0        0     1019 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/reports/cnv/AneuploidyScore.svelte
--rw-r--r--   0        0        0     1129 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/reports/cnv/AneuploidyScoreSummary.svelte
--rw-r--r--   0        0        0      466 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/reports/cnvkit/CNVkitDiagram.svelte
--rw-r--r--   0        0        0      518 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/reports/cnvkit/CNVkitHeatmap.svelte
--rw-r--r--   0        0        0      466 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/reports/cnvkit/CNVkitScatter.svelte
--rw-r--r--   0        0        0      404 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/reports/gsea/FGSEA.svelte
--rw-r--r--   0        0        0      416 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/reports/gsea/GSEA.svelte
--rw-r--r--   0        0        0      581 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/reports/scrna/CellsDistribution.svelte
--rw-r--r--   0        0        0      478 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/reports/scrna/DimPlots.svelte
--rw-r--r--   0        0        0      792 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/reports/scrna/GeneExpressionInvistigation.svelte
--rw-r--r--   0        0        0     1801 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/reports/scrna/MarkersFinder.svelte
--rw-r--r--   0        0        0     1040 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/reports/scrna/ScFGSEA.svelte
--rw-r--r--   0        0        0     4970 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/reports/scrna/SeuratClusterStats.svelte
--rw-r--r--   0        0        0     1180 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/reports/scrna/SeuratPreparing.svelte
--rw-r--r--   0        0        0      880 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/reports/scrna_metabolic_landscape/MetabolicFeatures.svelte
--rw-r--r--   0        0        0      992 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/reports/scrna_metabolic_landscape/MetabolicFeaturesIntraSubsets.svelte
--rw-r--r--   0        0        0     2542 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/reports/scrna_metabolic_landscape/MetabolicPathwayActivity.svelte
--rw-r--r--   0        0        0      636 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/reports/scrna_metabolic_landscape/MetabolicPathwayHeterogeneity.svelte
--rw-r--r--   0        0        0     2928 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/reports/tcr/CloneResidency.svelte
--rw-r--r--   0        0        0     7853 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/reports/tcr/Immunarch.svelte
--rw-r--r--   0        0        0     5523 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/reports/tcr/SampleDiversity.svelte
--rw-r--r--   0        0        0     3756 2023-03-08 21:55:11.748299 biopipen-0.8.0/biopipen/reports/tcr/TCRClusteringStats.svelte
--rw-r--r--   0        0        0      425 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/reports/tcr/VJUsage.svelte
--rw-r--r--   0        0        0     2626 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/reports/utils/gsea.liq
--rw-r--r--   0        0        0     1652 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/reports/utils/misc.liq
--rw-r--r--   0        0        0      576 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/reports/vcf/TruvariBenchSummary.svelte
--rw-r--r--   0        0        0      646 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/reports/vcf/TruvariConsistency.svelte
--rw-r--r--   0        0        0     5000 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/bam/CNAClinic.R
--rw-r--r--   0        0        0    12296 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/bam/CNVpytor.py
--rw-r--r--   0        0        0     3142 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/bam/ControlFREEC.py
--rw-r--r--   0        0        0     1343 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/bcftools/BcftoolsAnnotate.py
--rw-r--r--   0        0        0     2284 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/bcftools/BcftoolsFilter.py
--rw-r--r--   0        0        0      549 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/bcftools/BcftoolsSort.py
--rw-r--r--   0        0        0     4981 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/bed/Bed2Vcf.py
--rw-r--r--   0        0        0     6380 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/bed/BedConsensus.py
--rw-r--r--   0        0        0      256 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/bed/BedLiftOver.sh
--rw-r--r--   0        0        0     8078 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/cnv/AneuploidyScore.R
--rw-r--r--   0        0        0     4096 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/cnv/AneuploidyScoreSummary.R
--rw-r--r--   0        0        0      558 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/cnvkit/CNVkitAccess.py
--rw-r--r--   0        0        0     1496 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/cnvkit/CNVkitAutobin.py
--rw-r--r--   0        0        0     3596 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/cnvkit/CNVkitBatch.py
--rw-r--r--   0        0        0     2768 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/cnvkit/CNVkitCall.py
--rw-r--r--   0        0        0      679 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/cnvkit/CNVkitCoverage.py
--rw-r--r--   0        0        0     1681 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/cnvkit/CNVkitDiagram.py
--rw-r--r--   0        0        0      981 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/cnvkit/CNVkitFix.py
--rw-r--r--   0        0        0     1547 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/cnvkit/CNVkitGuessBaits.py
--rw-r--r--   0        0        0     2298 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/cnvkit/CNVkitHeatmap.py
--rw-r--r--   0        0        0     1253 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/cnvkit/CNVkitReference.py
--rw-r--r--   0        0        0     2394 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/cnvkit/CNVkitScatter.py
--rw-r--r--   0        0        0     1467 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/cnvkit/CNVkitSegment.py
--rw-r--r--   0        0        0    10586 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/cnvkit/guess_baits.py
--rw-r--r--   0        0        0     1880 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/gene/GeneNameConversion.py
--rw-r--r--   0        0        0      661 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/gsea/Enrichr.R
--rw-r--r--   0        0        0     1483 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/gsea/FGSEA.R
--rw-r--r--   0        0        0     1059 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/gsea/GSEA.R
--rw-r--r--   0        0        0     1356 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/gsea/PreRank.R
--rw-r--r--   0        0        0      440 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/misc/Config2File.py
--rw-r--r--   0        0        0      212 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/misc/Str2File.py
--rw-r--r--   0        0        0     1942 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/plot/Heatmap.R
--rw-r--r--   0        0        0      731 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/plot/VennDiagram.R
--rw-r--r--   0        0        0     1928 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/rnaseq/UnitConversion.R
--rw-r--r--   0        0        0      576 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna/CellTypeAnnotate-direct.R
--rw-r--r--   0        0        0     2547 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna/CellTypeAnnotate-sctype.R
--rw-r--r--   0        0        0      277 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna/CellTypeAnnotate.R
--rw-r--r--   0        0        0     2833 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna/CellsDistribution.R
--rw-r--r--   0        0        0     1513 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna/DimPlots.R
--rw-r--r--   0        0        0      605 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna/ExprImpute-alra.R
--rw-r--r--   0        0        0      624 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna/ExprImpute-rmagic.R
--rw-r--r--   0        0        0     1082 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna/ExprImpute-scimpute.R
--rw-r--r--   0        0        0      307 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna/ExprImpute.R
--rw-r--r--   0        0        0     3760 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna/GeneExpressionInvistigation.R
--rw-r--r--   0        0        0     4679 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna/MarkersFinder.R
--rw-r--r--   0        0        0     2958 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna/SCImpute.R
--rw-r--r--   0        0        0     4492 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna/ScFGSEA.R
--rw-r--r--   0        0        0    14656 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna/SeuratClusterStats.R
--rw-r--r--   0        0        0     5368 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna/SeuratClustering.R
--rw-r--r--   0        0        0      509 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna/SeuratFilter.R
--rw-r--r--   0        0        0      897 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna/SeuratLoading.R
--rw-r--r--   0        0        0      616 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna/SeuratMetadataMutater.R
--rw-r--r--   0        0        0     5304 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna/SeuratPreparing.R
--rw-r--r--   0        0        0      754 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna/SeuratSplit.R
--rw-r--r--   0        0        0     1776 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna/SeuratSubset.R
--rw-r--r--   0        0        0     2679 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna/Subset10X.R
--rw-r--r--   0        0        0      284 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna/Write10X.R
--rw-r--r--   0        0        0     5428 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna/sctype.R
--rw-r--r--   0        0        0     2942 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna_metabolic_landscape/MetabolicFeatures.R
--rw-r--r--   0        0        0     3570 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna_metabolic_landscape/MetabolicFeaturesIntraSubsets.R
--rw-r--r--   0        0        0    12083 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna_metabolic_landscape/MetabolicPathwayActivity.R
--rw-r--r--   0        0        0     7930 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/scrna_metabolic_landscape/MetabolicPathwayHeterogeneity.R
--rw-r--r--   0        0        0      672 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/tcgamaf/Maf2Vcf.py
--rw-r--r--   0        0        0      494 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/tcgamaf/MafAddChr.py
--rw-r--r--   0        0        0    22707 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/tcgamaf/maf2vcf.pl
--rw-r--r--   0        0        0     1315 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/tcr/Attach2Seurat.R
--rw-r--r--   0        0        0     9331 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/tcr/CloneResidency.R
--rw-r--r--   0        0        0     4527 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/tcr/CloneSizeQQPlot.R
--rw-r--r--   0        0        0    21251 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/tcr/Immunarch.R
--rw-r--r--   0        0        0      706 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/tcr/Immunarch2VDJtools.R
--rw-r--r--   0        0        0     3974 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/tcr/ImmunarchFilter.R
--rw-r--r--   0        0        0     4508 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/tcr/ImmunarchLoading.R
--rw-r--r--   0        0        0     1873 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/tcr/ImmunarchSplitIdents.R
--rw-r--r--   0        0        0     2603 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/tcr/SampleDiversity.R
--rw-r--r--   0        0        0     8351 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/tcr/TCRClustering.R
--rw-r--r--   0        0        0     7136 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/tcr/TCRClusteringStats.R
--rw-r--r--   0        0        0      437 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/tcr/VJUsage.R
--rw-r--r--   0        0        0      566 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/tcr/vdjtools-patch.sh
--rw-r--r--   0        0        0      765 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/vcf/TruvariBench.sh
--rw-r--r--   0        0        0     1474 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/vcf/TruvariBenchSummary.R
--rw-r--r--   0        0        0     2293 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/vcf/TruvariConsistency.R
--rw-r--r--   0        0        0      855 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/vcf/Vcf2Bed.py
--rw-r--r--   0        0        0      734 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/vcf/VcfAnno.py
--rw-r--r--   0        0        0      939 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/vcf/VcfDownSample.sh
--rw-r--r--   0        0        0     1881 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/vcf/VcfFilter.py
--rw-r--r--   0        0        0     1304 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/vcf/VcfFix.py
--rw-r--r--   0        0        0     2294 2023-03-08 21:55:11.752299 biopipen-0.8.0/biopipen/scripts/vcf/VcfFix_utils.py
--rw-r--r--   0        0        0      557 2023-03-08 21:55:11.756299 biopipen-0.8.0/biopipen/scripts/vcf/VcfIndex.py
--rw-r--r--   0        0        0      808 2023-03-08 21:55:11.756299 biopipen-0.8.0/biopipen/scripts/vcf/VcfIntersect.py
--rw-r--r--   0        0        0      562 2023-03-08 21:55:11.756299 biopipen-0.8.0/biopipen/scripts/vcf/VcfLiftOver.sh
--rw-r--r--   0        0        0     1275 2023-03-08 21:55:11.756299 biopipen-0.8.0/biopipen/scripts/vcf/VcfSplitSamples.py
--rw-r--r--   0        0        0      811 2023-03-08 21:55:11.756299 biopipen-0.8.0/biopipen/scripts/web/Download.py
--rw-r--r--   0        0        0     1017 2023-03-08 21:55:11.756299 biopipen-0.8.0/biopipen/scripts/web/DownloadList.py
--rw-r--r--   0        0        0     1243 2023-03-08 21:55:11.756299 biopipen-0.8.0/biopipen/utils/gene.R
--rw-r--r--   0        0        0     2246 2023-03-08 21:55:11.756299 biopipen-0.8.0/biopipen/utils/gene.py
--rw-r--r--   0        0        0     5794 2023-03-08 21:55:11.756299 biopipen-0.8.0/biopipen/utils/gsea.R
--rw-r--r--   0        0        0      537 2023-03-08 21:55:11.756299 biopipen-0.8.0/biopipen/utils/io.R
--rw-r--r--   0        0        0     2272 2023-03-08 21:55:11.756299 biopipen-0.8.0/biopipen/utils/misc.R
--rw-r--r--   0        0        0     4417 2023-03-08 21:55:11.756299 biopipen-0.8.0/biopipen/utils/plot.R
--rw-r--r--   0        0        0     3465 2023-03-08 21:55:11.756299 biopipen-0.8.0/biopipen/utils/reference.py
--rw-r--r--   0        0        0     1298 2023-03-08 21:55:11.756299 biopipen-0.8.0/biopipen/utils/rnaseq.R
--rw-r--r--   0        0        0     9377 2023-03-08 21:55:11.756299 biopipen-0.8.0/biopipen/utils/vcf.py
--rw-r--r--   0        0        0     1222 2023-03-08 21:55:11.756299 biopipen-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      839 1970-01-01 00:00:00.000000 biopipen-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/core/__init__.py
+-rw-r--r--   0        0        0     1069 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/core/config.py
+-rw-r--r--   0        0        0     1598 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/core/config.toml
+-rw-r--r--   0        0        0      344 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/core/defaults.py
+-rw-r--r--   0        0        0     2360 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/core/filters.py
+-rw-r--r--   0        0        0      498 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/core/proc.py
+-rw-r--r--   0        0        0     1586 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/core/testing.py
+-rw-r--r--   0        0        0        0 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/ns/__init__.py
+-rw-r--r--   0        0        0     6484 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/ns/bam.py
+-rw-r--r--   0        0        0     3467 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/ns/bcftools.py
+-rw-r--r--   0        0        0     5231 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/ns/bed.py
+-rw-r--r--   0        0        0     2901 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/ns/cnv.py
+-rw-r--r--   0        0        0    28348 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/ns/cnvkit.py
+-rw-r--r--   0        0        0    26835 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/ns/cnvkit_pipeline.py
+-rw-r--r--   0        0        0      484 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/ns/csv.py
+-rw-r--r--   0        0        0     2228 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/ns/gene.py
+-rw-r--r--   0        0        0     7423 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/ns/gsea.py
+-rw-r--r--   0        0        0     3015 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/ns/misc.py
+-rw-r--r--   0        0        0     4026 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/ns/plot.py
+-rw-r--r--   0        0        0      565 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/ns/rnaseq.py
+-rw-r--r--   0        0        0    28935 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/ns/scrna.py
+-rw-r--r--   0        0        0    15622 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/ns/scrna_metabolic_landscape.py
+-rw-r--r--   0        0        0     1455 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/ns/tcgamaf.py
+-rw-r--r--   0        0        0    23074 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/ns/tcr.py
+-rw-r--r--   0        0        0    15314 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/ns/vcf.py
+-rw-r--r--   0        0        0     2224 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/ns/web.py
+-rw-r--r--   0        0        0      212 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/bam/CNAClinic.svelte
+-rw-r--r--   0        0        0     1363 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/bam/CNVpytor.svelte
+-rw-r--r--   0        0        0      836 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/bam/ControlFREEC.svelte
+-rw-r--r--   0        0        0     1019 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/cnv/AneuploidyScore.svelte
+-rw-r--r--   0        0        0     1129 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/cnv/AneuploidyScoreSummary.svelte
+-rw-r--r--   0        0        0      466 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/cnvkit/CNVkitDiagram.svelte
+-rw-r--r--   0        0        0      518 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/cnvkit/CNVkitHeatmap.svelte
+-rw-r--r--   0        0        0      466 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/cnvkit/CNVkitScatter.svelte
+-rw-r--r--   0        0        0      404 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/gsea/FGSEA.svelte
+-rw-r--r--   0        0        0      416 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/gsea/GSEA.svelte
+-rw-r--r--   0        0        0      581 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/scrna/CellsDistribution.svelte
+-rw-r--r--   0        0        0      478 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/scrna/DimPlots.svelte
+-rw-r--r--   0        0        0      792 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/scrna/GeneExpressionInvistigation.svelte
+-rw-r--r--   0        0        0     1801 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/scrna/MarkersFinder.svelte
+-rw-r--r--   0        0        0     1040 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/scrna/ScFGSEA.svelte
+-rw-r--r--   0        0        0     4970 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/scrna/SeuratClusterStats.svelte
+-rw-r--r--   0        0        0     1180 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/scrna/SeuratPreparing.svelte
+-rw-r--r--   0        0        0      880 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/scrna_metabolic_landscape/MetabolicFeatures.svelte
+-rw-r--r--   0        0        0      992 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/scrna_metabolic_landscape/MetabolicFeaturesIntraSubsets.svelte
+-rw-r--r--   0        0        0     2542 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/scrna_metabolic_landscape/MetabolicPathwayActivity.svelte
+-rw-r--r--   0        0        0      636 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/scrna_metabolic_landscape/MetabolicPathwayHeterogeneity.svelte
+-rw-r--r--   0        0        0     2928 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/tcr/CloneResidency.svelte
+-rw-r--r--   0        0        0     7853 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/tcr/Immunarch.svelte
+-rw-r--r--   0        0        0     5523 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/tcr/SampleDiversity.svelte
+-rw-r--r--   0        0        0     3756 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/tcr/TCRClusteringStats.svelte
+-rw-r--r--   0        0        0      425 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/tcr/VJUsage.svelte
+-rw-r--r--   0        0        0     2626 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/utils/gsea.liq
+-rw-r--r--   0        0        0     1652 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/utils/misc.liq
+-rw-r--r--   0        0        0      576 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/vcf/TruvariBenchSummary.svelte
+-rw-r--r--   0        0        0      646 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/reports/vcf/TruvariConsistency.svelte
+-rw-r--r--   0        0        0     5000 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/scripts/bam/CNAClinic.R
+-rw-r--r--   0        0        0    12296 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/scripts/bam/CNVpytor.py
+-rw-r--r--   0        0        0     3142 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/scripts/bam/ControlFREEC.py
+-rw-r--r--   0        0        0     1343 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/scripts/bcftools/BcftoolsAnnotate.py
+-rw-r--r--   0        0        0     2284 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/scripts/bcftools/BcftoolsFilter.py
+-rw-r--r--   0        0        0      549 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/scripts/bcftools/BcftoolsSort.py
+-rw-r--r--   0        0        0     4981 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/scripts/bed/Bed2Vcf.py
+-rw-r--r--   0        0        0     6380 2023-03-11 04:24:51.172354 biopipen-0.9.0/biopipen/scripts/bed/BedConsensus.py
+-rw-r--r--   0        0        0      256 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/bed/BedLiftOver.sh
+-rw-r--r--   0        0        0     8078 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/cnv/AneuploidyScore.R
+-rw-r--r--   0        0        0     4096 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/cnv/AneuploidyScoreSummary.R
+-rw-r--r--   0        0        0      558 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/cnvkit/CNVkitAccess.py
+-rw-r--r--   0        0        0     1496 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/cnvkit/CNVkitAutobin.py
+-rw-r--r--   0        0        0     3596 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/cnvkit/CNVkitBatch.py
+-rw-r--r--   0        0        0     2768 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/cnvkit/CNVkitCall.py
+-rw-r--r--   0        0        0      679 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/cnvkit/CNVkitCoverage.py
+-rw-r--r--   0        0        0     1681 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/cnvkit/CNVkitDiagram.py
+-rw-r--r--   0        0        0      981 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/cnvkit/CNVkitFix.py
+-rw-r--r--   0        0        0     1547 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/cnvkit/CNVkitGuessBaits.py
+-rw-r--r--   0        0        0     2298 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/cnvkit/CNVkitHeatmap.py
+-rw-r--r--   0        0        0     1253 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/cnvkit/CNVkitReference.py
+-rw-r--r--   0        0        0     2394 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/cnvkit/CNVkitScatter.py
+-rw-r--r--   0        0        0     1467 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/cnvkit/CNVkitSegment.py
+-rw-r--r--   0        0        0    10586 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/cnvkit/guess_baits.py
+-rw-r--r--   0        0        0     1880 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/gene/GeneNameConversion.py
+-rw-r--r--   0        0        0      661 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/gsea/Enrichr.R
+-rw-r--r--   0        0        0     1483 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/gsea/FGSEA.R
+-rw-r--r--   0        0        0     1059 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/gsea/GSEA.R
+-rw-r--r--   0        0        0     1356 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/gsea/PreRank.R
+-rw-r--r--   0        0        0      440 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/misc/Config2File.py
+-rw-r--r--   0        0        0      212 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/misc/Str2File.py
+-rw-r--r--   0        0        0     1942 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/plot/Heatmap.R
+-rw-r--r--   0        0        0      731 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/plot/VennDiagram.R
+-rw-r--r--   0        0        0     1928 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/rnaseq/UnitConversion.R
+-rw-r--r--   0        0        0      576 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna/CellTypeAnnotate-direct.R
+-rw-r--r--   0        0        0     2547 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna/CellTypeAnnotate-sctype.R
+-rw-r--r--   0        0        0      277 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna/CellTypeAnnotate.R
+-rw-r--r--   0        0        0     2833 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna/CellsDistribution.R
+-rw-r--r--   0        0        0     1513 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna/DimPlots.R
+-rw-r--r--   0        0        0      605 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna/ExprImpute-alra.R
+-rw-r--r--   0        0        0      624 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna/ExprImpute-rmagic.R
+-rw-r--r--   0        0        0     1082 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna/ExprImpute-scimpute.R
+-rw-r--r--   0        0        0      307 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna/ExprImpute.R
+-rw-r--r--   0        0        0     3760 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna/GeneExpressionInvistigation.R
+-rw-r--r--   0        0        0     4679 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna/MarkersFinder.R
+-rw-r--r--   0        0        0     2958 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna/SCImpute.R
+-rw-r--r--   0        0        0     4492 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna/ScFGSEA.R
+-rw-r--r--   0        0        0    14656 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna/SeuratClusterStats.R
+-rw-r--r--   0        0        0     5368 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna/SeuratClustering.R
+-rw-r--r--   0        0        0      509 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna/SeuratFilter.R
+-rw-r--r--   0        0        0      897 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna/SeuratLoading.R
+-rw-r--r--   0        0        0      616 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna/SeuratMetadataMutater.R
+-rw-r--r--   0        0        0     5304 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna/SeuratPreparing.R
+-rw-r--r--   0        0        0      754 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna/SeuratSplit.R
+-rw-r--r--   0        0        0     1776 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna/SeuratSubset.R
+-rw-r--r--   0        0        0     2679 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna/Subset10X.R
+-rw-r--r--   0        0        0      284 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna/Write10X.R
+-rw-r--r--   0        0        0     5428 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna/sctype.R
+-rw-r--r--   0        0        0     2942 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna_metabolic_landscape/MetabolicFeatures.R
+-rw-r--r--   0        0        0     3570 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna_metabolic_landscape/MetabolicFeaturesIntraSubsets.R
+-rw-r--r--   0        0        0    12083 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna_metabolic_landscape/MetabolicPathwayActivity.R
+-rw-r--r--   0        0        0     7930 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/scrna_metabolic_landscape/MetabolicPathwayHeterogeneity.R
+-rw-r--r--   0        0        0      672 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/tcgamaf/Maf2Vcf.py
+-rw-r--r--   0        0        0      494 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/tcgamaf/MafAddChr.py
+-rw-r--r--   0        0        0    22707 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/tcgamaf/maf2vcf.pl
+-rw-r--r--   0        0        0     1315 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/tcr/Attach2Seurat.R
+-rw-r--r--   0        0        0     9331 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/tcr/CloneResidency.R
+-rw-r--r--   0        0        0     4527 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/tcr/CloneSizeQQPlot.R
+-rw-r--r--   0        0        0    21251 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/tcr/Immunarch.R
+-rw-r--r--   0        0        0      706 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/tcr/Immunarch2VDJtools.R
+-rw-r--r--   0        0        0     3974 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/tcr/ImmunarchFilter.R
+-rw-r--r--   0        0        0     4508 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/tcr/ImmunarchLoading.R
+-rw-r--r--   0        0        0     1873 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/tcr/ImmunarchSplitIdents.R
+-rw-r--r--   0        0        0     2603 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/tcr/SampleDiversity.R
+-rw-r--r--   0        0        0     8351 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/tcr/TCRClustering.R
+-rw-r--r--   0        0        0     7136 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/tcr/TCRClusteringStats.R
+-rw-r--r--   0        0        0      437 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/tcr/VJUsage.R
+-rw-r--r--   0        0        0      566 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/tcr/vdjtools-patch.sh
+-rw-r--r--   0        0        0      765 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/vcf/TruvariBench.sh
+-rw-r--r--   0        0        0     1474 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/vcf/TruvariBenchSummary.R
+-rw-r--r--   0        0        0     2293 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/vcf/TruvariConsistency.R
+-rw-r--r--   0        0        0      855 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/vcf/Vcf2Bed.py
+-rw-r--r--   0        0        0      734 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/vcf/VcfAnno.py
+-rw-r--r--   0        0        0      939 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/vcf/VcfDownSample.sh
+-rw-r--r--   0        0        0     1881 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/vcf/VcfFilter.py
+-rw-r--r--   0        0        0     1304 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/vcf/VcfFix.py
+-rw-r--r--   0        0        0     2294 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/vcf/VcfFix_utils.py
+-rw-r--r--   0        0        0      557 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/vcf/VcfIndex.py
+-rw-r--r--   0        0        0      808 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/vcf/VcfIntersect.py
+-rw-r--r--   0        0        0      562 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/vcf/VcfLiftOver.sh
+-rw-r--r--   0        0        0     1275 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/vcf/VcfSplitSamples.py
+-rw-r--r--   0        0        0      811 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/web/Download.py
+-rw-r--r--   0        0        0     1017 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/scripts/web/DownloadList.py
+-rw-r--r--   0        0        0     1243 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/utils/gene.R
+-rw-r--r--   0        0        0     2246 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/utils/gene.py
+-rw-r--r--   0        0        0     5794 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/utils/gsea.R
+-rw-r--r--   0        0        0      537 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/utils/io.R
+-rw-r--r--   0        0        0     2272 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/utils/misc.R
+-rw-r--r--   0        0        0     4417 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/utils/plot.R
+-rw-r--r--   0        0        0     3465 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/utils/reference.py
+-rw-r--r--   0        0        0     1298 2023-03-11 04:24:51.176354 biopipen-0.9.0/biopipen/utils/rnaseq.R
+-rw-r--r--   0        0        0     9377 2023-03-11 04:24:51.180354 biopipen-0.9.0/biopipen/utils/vcf.py
+-rw-r--r--   0        0        0     1222 2023-03-11 04:24:51.180354 biopipen-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      839 1970-01-01 00:00:00.000000 biopipen-0.9.0/PKG-INFO
```

### Comparing `biopipen-0.8.0/biopipen/core/config.py` & `biopipen-0.9.0/biopipen/core/config.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/core/config.toml` & `biopipen-0.9.0/biopipen/core/config.toml`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/core/filters.py` & `biopipen-0.9.0/biopipen/core/filters.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/core/testing.py` & `biopipen-0.9.0/biopipen/core/testing.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/ns/bam.py` & `biopipen-0.9.0/biopipen/ns/bam.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/ns/bcftools.py` & `biopipen-0.9.0/biopipen/ns/bcftools.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/ns/bed.py` & `biopipen-0.9.0/biopipen/ns/bed.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/ns/cnv.py` & `biopipen-0.9.0/biopipen/ns/cnv.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/ns/cnvkit.py` & `biopipen-0.9.0/biopipen/ns/cnvkit.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/ns/cnvkit_pipeline.py` & `biopipen-0.9.0/biopipen/ns/cnvkit_pipeline.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/ns/gene.py` & `biopipen-0.9.0/biopipen/ns/gene.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/ns/gsea.py` & `biopipen-0.9.0/biopipen/ns/gsea.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/ns/misc.py` & `biopipen-0.9.0/biopipen/ns/misc.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/ns/plot.py` & `biopipen-0.9.0/biopipen/ns/plot.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/ns/rnaseq.py` & `biopipen-0.9.0/biopipen/ns/rnaseq.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/ns/scrna.py` & `biopipen-0.9.0/biopipen/ns/scrna.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/ns/scrna_metabolic_landscape.py` & `biopipen-0.9.0/biopipen/ns/scrna_metabolic_landscape.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/ns/tcgamaf.py` & `biopipen-0.9.0/biopipen/ns/tcgamaf.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/ns/tcr.py` & `biopipen-0.9.0/biopipen/ns/tcr.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/ns/vcf.py` & `biopipen-0.9.0/biopipen/ns/vcf.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/ns/web.py` & `biopipen-0.9.0/biopipen/ns/web.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/reports/bam/CNVpytor.svelte` & `biopipen-0.9.0/biopipen/reports/bam/CNVpytor.svelte`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/reports/bam/ControlFREEC.svelte` & `biopipen-0.9.0/biopipen/reports/bam/ControlFREEC.svelte`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/reports/cnv/AneuploidyScore.svelte` & `biopipen-0.9.0/biopipen/reports/cnv/AneuploidyScore.svelte`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/reports/cnv/AneuploidyScoreSummary.svelte` & `biopipen-0.9.0/biopipen/reports/cnv/AneuploidyScoreSummary.svelte`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/reports/cnvkit/CNVkitHeatmap.svelte` & `biopipen-0.9.0/biopipen/reports/cnvkit/CNVkitHeatmap.svelte`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/reports/scrna/CellsDistribution.svelte` & `biopipen-0.9.0/biopipen/reports/scrna/CellsDistribution.svelte`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/reports/scrna/GeneExpressionInvistigation.svelte` & `biopipen-0.9.0/biopipen/reports/scrna/GeneExpressionInvistigation.svelte`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/reports/scrna/MarkersFinder.svelte` & `biopipen-0.9.0/biopipen/reports/scrna/MarkersFinder.svelte`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/reports/scrna/ScFGSEA.svelte` & `biopipen-0.9.0/biopipen/reports/scrna/ScFGSEA.svelte`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/reports/scrna/SeuratClusterStats.svelte` & `biopipen-0.9.0/biopipen/reports/scrna/SeuratClusterStats.svelte`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/reports/scrna/SeuratPreparing.svelte` & `biopipen-0.9.0/biopipen/reports/scrna/SeuratPreparing.svelte`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/reports/scrna_metabolic_landscape/MetabolicFeatures.svelte` & `biopipen-0.9.0/biopipen/reports/scrna_metabolic_landscape/MetabolicFeatures.svelte`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/reports/scrna_metabolic_landscape/MetabolicFeaturesIntraSubsets.svelte` & `biopipen-0.9.0/biopipen/reports/scrna_metabolic_landscape/MetabolicFeaturesIntraSubsets.svelte`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/reports/scrna_metabolic_landscape/MetabolicPathwayActivity.svelte` & `biopipen-0.9.0/biopipen/reports/scrna_metabolic_landscape/MetabolicPathwayActivity.svelte`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/reports/scrna_metabolic_landscape/MetabolicPathwayHeterogeneity.svelte` & `biopipen-0.9.0/biopipen/reports/scrna_metabolic_landscape/MetabolicPathwayHeterogeneity.svelte`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/reports/tcr/CloneResidency.svelte` & `biopipen-0.9.0/biopipen/reports/tcr/CloneResidency.svelte`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/reports/tcr/Immunarch.svelte` & `biopipen-0.9.0/biopipen/reports/tcr/Immunarch.svelte`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/reports/tcr/SampleDiversity.svelte` & `biopipen-0.9.0/biopipen/reports/tcr/SampleDiversity.svelte`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/reports/tcr/TCRClusteringStats.svelte` & `biopipen-0.9.0/biopipen/reports/tcr/TCRClusteringStats.svelte`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/reports/utils/gsea.liq` & `biopipen-0.9.0/biopipen/reports/utils/gsea.liq`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/reports/utils/misc.liq` & `biopipen-0.9.0/biopipen/reports/utils/misc.liq`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/reports/vcf/TruvariBenchSummary.svelte` & `biopipen-0.9.0/biopipen/reports/vcf/TruvariBenchSummary.svelte`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/reports/vcf/TruvariConsistency.svelte` & `biopipen-0.9.0/biopipen/reports/vcf/TruvariConsistency.svelte`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/bam/CNAClinic.R` & `biopipen-0.9.0/biopipen/scripts/bam/CNAClinic.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/bam/CNVpytor.py` & `biopipen-0.9.0/biopipen/scripts/bam/CNVpytor.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/bam/ControlFREEC.py` & `biopipen-0.9.0/biopipen/scripts/bam/ControlFREEC.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/bcftools/BcftoolsAnnotate.py` & `biopipen-0.9.0/biopipen/scripts/bcftools/BcftoolsAnnotate.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/bcftools/BcftoolsFilter.py` & `biopipen-0.9.0/biopipen/scripts/bcftools/BcftoolsFilter.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/bcftools/BcftoolsSort.py` & `biopipen-0.9.0/biopipen/scripts/bcftools/BcftoolsSort.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/bed/Bed2Vcf.py` & `biopipen-0.9.0/biopipen/scripts/bed/Bed2Vcf.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/bed/BedConsensus.py` & `biopipen-0.9.0/biopipen/scripts/bed/BedConsensus.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/cnv/AneuploidyScore.R` & `biopipen-0.9.0/biopipen/scripts/cnv/AneuploidyScore.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/cnv/AneuploidyScoreSummary.R` & `biopipen-0.9.0/biopipen/scripts/cnv/AneuploidyScoreSummary.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/cnvkit/CNVkitAccess.py` & `biopipen-0.9.0/biopipen/scripts/cnvkit/CNVkitAccess.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/cnvkit/CNVkitAutobin.py` & `biopipen-0.9.0/biopipen/scripts/cnvkit/CNVkitAutobin.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/cnvkit/CNVkitBatch.py` & `biopipen-0.9.0/biopipen/scripts/cnvkit/CNVkitBatch.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/cnvkit/CNVkitCall.py` & `biopipen-0.9.0/biopipen/scripts/cnvkit/CNVkitCall.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/cnvkit/CNVkitCoverage.py` & `biopipen-0.9.0/biopipen/scripts/cnvkit/CNVkitCoverage.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/cnvkit/CNVkitDiagram.py` & `biopipen-0.9.0/biopipen/scripts/cnvkit/CNVkitDiagram.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/cnvkit/CNVkitFix.py` & `biopipen-0.9.0/biopipen/scripts/cnvkit/CNVkitFix.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/cnvkit/CNVkitGuessBaits.py` & `biopipen-0.9.0/biopipen/scripts/cnvkit/CNVkitGuessBaits.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/cnvkit/CNVkitHeatmap.py` & `biopipen-0.9.0/biopipen/scripts/cnvkit/CNVkitHeatmap.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/cnvkit/CNVkitReference.py` & `biopipen-0.9.0/biopipen/scripts/cnvkit/CNVkitReference.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/cnvkit/CNVkitScatter.py` & `biopipen-0.9.0/biopipen/scripts/cnvkit/CNVkitScatter.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/cnvkit/CNVkitSegment.py` & `biopipen-0.9.0/biopipen/scripts/cnvkit/CNVkitSegment.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/cnvkit/guess_baits.py` & `biopipen-0.9.0/biopipen/scripts/cnvkit/guess_baits.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/gene/GeneNameConversion.py` & `biopipen-0.9.0/biopipen/scripts/gene/GeneNameConversion.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/gsea/Enrichr.R` & `biopipen-0.9.0/biopipen/scripts/gsea/Enrichr.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/gsea/FGSEA.R` & `biopipen-0.9.0/biopipen/scripts/gsea/FGSEA.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/gsea/GSEA.R` & `biopipen-0.9.0/biopipen/scripts/gsea/GSEA.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/gsea/PreRank.R` & `biopipen-0.9.0/biopipen/scripts/gsea/PreRank.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/plot/Heatmap.R` & `biopipen-0.9.0/biopipen/scripts/plot/Heatmap.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/plot/VennDiagram.R` & `biopipen-0.9.0/biopipen/scripts/plot/VennDiagram.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/rnaseq/UnitConversion.R` & `biopipen-0.9.0/biopipen/scripts/rnaseq/UnitConversion.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/scrna/CellTypeAnnotate-direct.R` & `biopipen-0.9.0/biopipen/scripts/scrna/CellTypeAnnotate-direct.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/scrna/CellTypeAnnotate-sctype.R` & `biopipen-0.9.0/biopipen/scripts/scrna/CellTypeAnnotate-sctype.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/scrna/CellsDistribution.R` & `biopipen-0.9.0/biopipen/scripts/scrna/CellsDistribution.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/scrna/DimPlots.R` & `biopipen-0.9.0/biopipen/scripts/scrna/DimPlots.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/scrna/ExprImpute-alra.R` & `biopipen-0.9.0/biopipen/scripts/scrna/ExprImpute-alra.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/scrna/ExprImpute-rmagic.R` & `biopipen-0.9.0/biopipen/scripts/scrna/ExprImpute-rmagic.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/scrna/ExprImpute-scimpute.R` & `biopipen-0.9.0/biopipen/scripts/scrna/ExprImpute-scimpute.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/scrna/GeneExpressionInvistigation.R` & `biopipen-0.9.0/biopipen/scripts/scrna/GeneExpressionInvistigation.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/scrna/MarkersFinder.R` & `biopipen-0.9.0/biopipen/scripts/scrna/MarkersFinder.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/scrna/SCImpute.R` & `biopipen-0.9.0/biopipen/scripts/scrna/SCImpute.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/scrna/ScFGSEA.R` & `biopipen-0.9.0/biopipen/scripts/scrna/ScFGSEA.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/scrna/SeuratClusterStats.R` & `biopipen-0.9.0/biopipen/scripts/scrna/SeuratClusterStats.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/scrna/SeuratClustering.R` & `biopipen-0.9.0/biopipen/scripts/scrna/SeuratClustering.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/scrna/SeuratLoading.R` & `biopipen-0.9.0/biopipen/scripts/scrna/SeuratLoading.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/scrna/SeuratMetadataMutater.R` & `biopipen-0.9.0/biopipen/scripts/scrna/SeuratMetadataMutater.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/scrna/SeuratPreparing.R` & `biopipen-0.9.0/biopipen/scripts/scrna/SeuratPreparing.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/scrna/SeuratSplit.R` & `biopipen-0.9.0/biopipen/scripts/scrna/SeuratSplit.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/scrna/SeuratSubset.R` & `biopipen-0.9.0/biopipen/scripts/scrna/SeuratSubset.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/scrna/Subset10X.R` & `biopipen-0.9.0/biopipen/scripts/scrna/Subset10X.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/scrna/sctype.R` & `biopipen-0.9.0/biopipen/scripts/scrna/sctype.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/scrna_metabolic_landscape/MetabolicFeatures.R` & `biopipen-0.9.0/biopipen/scripts/scrna_metabolic_landscape/MetabolicFeatures.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/scrna_metabolic_landscape/MetabolicFeaturesIntraSubsets.R` & `biopipen-0.9.0/biopipen/scripts/scrna_metabolic_landscape/MetabolicFeaturesIntraSubsets.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/scrna_metabolic_landscape/MetabolicPathwayActivity.R` & `biopipen-0.9.0/biopipen/scripts/scrna_metabolic_landscape/MetabolicPathwayActivity.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/scrna_metabolic_landscape/MetabolicPathwayHeterogeneity.R` & `biopipen-0.9.0/biopipen/scripts/scrna_metabolic_landscape/MetabolicPathwayHeterogeneity.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/tcgamaf/Maf2Vcf.py` & `biopipen-0.9.0/biopipen/scripts/tcgamaf/Maf2Vcf.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/tcgamaf/maf2vcf.pl` & `biopipen-0.9.0/biopipen/scripts/tcgamaf/maf2vcf.pl`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/tcr/Attach2Seurat.R` & `biopipen-0.9.0/biopipen/scripts/tcr/Attach2Seurat.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/tcr/CloneResidency.R` & `biopipen-0.9.0/biopipen/scripts/tcr/CloneResidency.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/tcr/CloneSizeQQPlot.R` & `biopipen-0.9.0/biopipen/scripts/tcr/CloneSizeQQPlot.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/tcr/Immunarch.R` & `biopipen-0.9.0/biopipen/scripts/tcr/Immunarch.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/tcr/Immunarch2VDJtools.R` & `biopipen-0.9.0/biopipen/scripts/tcr/Immunarch2VDJtools.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/tcr/ImmunarchFilter.R` & `biopipen-0.9.0/biopipen/scripts/tcr/ImmunarchFilter.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/tcr/ImmunarchLoading.R` & `biopipen-0.9.0/biopipen/scripts/tcr/ImmunarchLoading.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/tcr/ImmunarchSplitIdents.R` & `biopipen-0.9.0/biopipen/scripts/tcr/ImmunarchSplitIdents.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/tcr/SampleDiversity.R` & `biopipen-0.9.0/biopipen/scripts/tcr/SampleDiversity.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/tcr/TCRClustering.R` & `biopipen-0.9.0/biopipen/scripts/tcr/TCRClustering.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/tcr/TCRClusteringStats.R` & `biopipen-0.9.0/biopipen/scripts/tcr/TCRClusteringStats.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/tcr/vdjtools-patch.sh` & `biopipen-0.9.0/biopipen/scripts/tcr/vdjtools-patch.sh`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/vcf/TruvariBench.sh` & `biopipen-0.9.0/biopipen/scripts/vcf/TruvariBench.sh`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/vcf/TruvariBenchSummary.R` & `biopipen-0.9.0/biopipen/scripts/vcf/TruvariBenchSummary.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/vcf/TruvariConsistency.R` & `biopipen-0.9.0/biopipen/scripts/vcf/TruvariConsistency.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/vcf/Vcf2Bed.py` & `biopipen-0.9.0/biopipen/scripts/vcf/Vcf2Bed.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/vcf/VcfAnno.py` & `biopipen-0.9.0/biopipen/scripts/vcf/VcfAnno.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/vcf/VcfDownSample.sh` & `biopipen-0.9.0/biopipen/scripts/vcf/VcfDownSample.sh`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/vcf/VcfFilter.py` & `biopipen-0.9.0/biopipen/scripts/vcf/VcfFilter.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/vcf/VcfFix.py` & `biopipen-0.9.0/biopipen/scripts/vcf/VcfFix.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/vcf/VcfFix_utils.py` & `biopipen-0.9.0/biopipen/scripts/vcf/VcfFix_utils.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/vcf/VcfIndex.py` & `biopipen-0.9.0/biopipen/scripts/vcf/VcfIndex.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/vcf/VcfIntersect.py` & `biopipen-0.9.0/biopipen/scripts/vcf/VcfIntersect.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/vcf/VcfLiftOver.sh` & `biopipen-0.9.0/biopipen/scripts/vcf/VcfLiftOver.sh`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/vcf/VcfSplitSamples.py` & `biopipen-0.9.0/biopipen/scripts/vcf/VcfSplitSamples.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/web/Download.py` & `biopipen-0.9.0/biopipen/scripts/web/Download.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/scripts/web/DownloadList.py` & `biopipen-0.9.0/biopipen/scripts/web/DownloadList.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/utils/gene.R` & `biopipen-0.9.0/biopipen/utils/gene.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/utils/gene.py` & `biopipen-0.9.0/biopipen/utils/gene.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/utils/gsea.R` & `biopipen-0.9.0/biopipen/utils/gsea.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/utils/io.R` & `biopipen-0.9.0/biopipen/utils/io.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/utils/misc.R` & `biopipen-0.9.0/biopipen/utils/misc.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/utils/plot.R` & `biopipen-0.9.0/biopipen/utils/plot.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/utils/reference.py` & `biopipen-0.9.0/biopipen/utils/reference.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/utils/rnaseq.R` & `biopipen-0.9.0/biopipen/utils/rnaseq.R`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/biopipen/utils/vcf.py` & `biopipen-0.9.0/biopipen/utils/vcf.py`

 * *Files identical despite different names*

### Comparing `biopipen-0.8.0/pyproject.toml` & `biopipen-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "biopipen"
-version = "0.8.0"
+version = "0.9.0"
 description = "Bioinformatics processes/pipelines that can be run from `pipen run`"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
-pipen = "^0.5"
-pipen-filters = "^0.4"
-pipen-report = "^0.6"
-pipen-cli-run = "^0.5"
-pipen-verbose = "^0.3"
-pipen-args = "^0.6"
+pipen = "^0.6"
+pipen-filters = "^0.5"
+pipen-report = "^0.7"
+pipen-cli-run = "^0.6"
+pipen-verbose = "^0.4"
+pipen-args = "^0.7"
 cmdy = "^0.5"
 datar = {version = "^0.11", extras = ["pandas"]}
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.plugins.pipen_cli_run]
 bam = "biopipen.ns.bam"
```

### Comparing `biopipen-0.8.0/PKG-INFO` & `biopipen-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: biopipen
-Version: 0.8.0
+Version: 0.9.0
 Summary: Bioinformatics processes/pipelines that can be run from `pipen run`
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cmdy (>=0.5,<0.6)
 Requires-Dist: datar[pandas] (>=0.11,<0.12)
-Requires-Dist: pipen (>=0.5,<0.6)
-Requires-Dist: pipen-args (>=0.6,<0.7)
-Requires-Dist: pipen-cli-run (>=0.5,<0.6)
-Requires-Dist: pipen-filters (>=0.4,<0.5)
-Requires-Dist: pipen-report (>=0.6,<0.7)
-Requires-Dist: pipen-verbose (>=0.3,<0.4)
+Requires-Dist: pipen (>=0.6,<0.7)
+Requires-Dist: pipen-args (>=0.7,<0.8)
+Requires-Dist: pipen-cli-run (>=0.6,<0.7)
+Requires-Dist: pipen-filters (>=0.5,<0.6)
+Requires-Dist: pipen-report (>=0.7,<0.8)
+Requires-Dist: pipen-verbose (>=0.4,<0.5)
```

