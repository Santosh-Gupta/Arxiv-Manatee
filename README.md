<p align="center">
  <img src="https://snag.gy/cwnUGB.jpg">
</p>


To do

### -Develop dataset (in progress)

### -Figure out how to process data for training

https://github.com/yaserkl/RLSeq2Seq/tree/master/src/helper

### -Train summarizer using this repo

https://github.com/yaserkl/RLSeq2Seq

### -Download Arxiv papers from cs.[CV|CL|LG|AI|NE]/stat.ML 

https://arxiv.org/help/bulk_data

Should be around ~73000 papers

The Arxiv-Sanity github repo may help figure out how to do this

https://github.com/karpathy/arxiv-sanity-preserver/blob/master/fetch_papers.py

### -Find best solution to retieving on-disk text data using index or key.

Possible solution 1: sqlite

Possible solution 2. pickledb https://pythonhosted.org/pickleDB/

Pssible solution 3. sqlitedict https://pypi.org/project/sqlitedict/

### -Take text from extracted Arxiv papers and seperate them into sections/paragraph. Store each section/paragraph as a row in a row in a sqlite database. Should also contain Title, and arxiv link as seperate rows. Possibly abstract as well. 

Possibly helpful resources

https://github.com/karpathy/arxiv-sanity-preserver/blob/master/parse_pdf_to_text.py

https://github.com/arxiv-vanity

https://github.com/arxiv-vanity/engrafo

### -Figure out most efficient way to do embedding similarity search for large amounts of data. 

Possible solutions 1 search through hdf5 data stored on disk

Possible solution 2 use Faiss IVF65536_HNSW32 index https://github.com/facebookresearch/faiss/wiki/Guidelines-to-choose-an-index
