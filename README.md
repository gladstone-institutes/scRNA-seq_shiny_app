# scRNA-seq_shiny_app
R Shiny application for scRNA-seq


### To downsize your Seurat Object, you can remove nonessential data (Without affecting FeaturPlot. Other functions haven't been tested yet):

yourSeuratObject$nCount_RNA=NA
yourSeuratObject$nFeature_RNA=NA
yourSeuratObject$integrated_snn_res.0.3=NA
yourSeuratObject$seurat_clusters=NA
yourSeuratObject@assays$integrated=NA
yourSeuratObject@meta.data$nCount_RNA=NA
yourSeuratObject@meta.data$nFeature_RNA=NA
yourSeuratObject@meta.data$integrated_snn_res.0.3=NA
yourSeuratObject@meta.data$seurat_clusters=NA
yourSeuratObject@graphs$integrated_nn=NA
yourSeuratObject@graphs$integrated_snn=NA
yourSeuratObject@reductions$pca=NA
yourSeuratObject@tools$Integration=NA
