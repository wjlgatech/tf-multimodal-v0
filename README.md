# tf-multimodal

## Objectives

To build a automated Tensorflow based multimodal classifier that consumes tabular data with cnt, cat, txt, img columns.

## Milestones
- [5/5] build a working [notebook](https://github.com/wjlgatech/tf-multimodal/blob/main/tf_multimodal.ipynb) with 1 sample dataset
- [/5] test performance on other datasets
- [/5] modularize it and put in .py
- [/5] packaging it into a library

## Features

**Features Built**
- [5/5] emb cnt_cols

- [5/5] emb cat_cols

- [5/5] emb txt_cols

- [5/5] automate the separation for cnt, cat, txt columns in df

- [5/5] OneTower structure: concat the emb of txt_cols, cnt_cols, cat_cols for df

- [5/5] allow txt_, cnt_, cat_cols interaction with deep cross module

**Features to Build**

- [/5] trace feature contribution/importance with col_emb_ls

- [/5] tf_clf model based feature selection

- [/5] hyperparameter tuning

- [/5] modularize get_txt_emb_layer(), follow by txt_post_processing such as LSTM, RNN, seq2seq, BERT, https://www.tensorflow.org/text/tutorials/classify_text_with_bert

- [/5] TwoTower structure: concat the emb of txt_cols, cnt_cols, cat_cols for user and item, respectively. It will be useful in a hybrid recommendation system.

- [/5] emb img_cols

- [/5] concat emb of cnt + cat + txt + img, integrate info in smart ways

**References & Credits**:

- tf cnt+cat: https://www.tensorflow.org/tutorials/structured_data/preprocessing_layers

- cat + img: https://www.pyimagesearch.com/2019/02/04/keras-multiple-inputs-and-mixed-data/

- cnt + txt: https://towardsdatascience.com/combining-numerical-and-text-features-in-deep-neural-networks-e91f0237eea4

- txt bert https://www.tensorflow.org/text/tutorials/classify_text_with_bert
