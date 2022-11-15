# Hebrew OCR improvement
## Idea
There are many Jewish texts, which is in bad condition and can not be processed with OCR algoritms. So I trained DE-GAN model on prepared jewish texts dataset.
## Data 
Data is Talmud pages, scrapped from https://www.daf-yomi.com/ with `Selenium`. After that data is processed with `pdfplumber`,`OpenCV` and `augraphy` in order to get 256x256 grayscale image pairs of bad and good text.
## Model
I used `DE-GAN` model, proposed by Mohamed Ali Souibgui and Yousri Kessentini(2020).
## Reference
Souibgui, A., & Kessentini, Y.(2020) *DE-GAN: A Conditional Generative Adversarial Network for Document Enhancement*. Retrieved from https://arxiv.org/pdf/2010.08764.pdf