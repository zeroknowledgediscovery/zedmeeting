
Submitted the LSM survey paper to Science advances journal today on Sep 30. 

Will be submitting the AJE paper after incorporating the CTAB-GAN synthetic data generator on Friday (Oct 02).

Some details while running the LSM code on the genomic data with one column. 

import fitz
import argparse

def pdf_to_markdown(pdf_path, md_path):
    doc = fitz.open(pdf_path)

    with open(md_path, "w", encoding="utf-8") as f:
        for page_num, page in enumerate(doc, start=1):
            text = page.get_text("text")

            f.write(f"\n\n<!-- PAGE {page_num} -->\n\n")
            f.write(text)

    print(f"Saved: {md_path}")


if __name__ == "__main__":
    parser = argparse.ArgumentParser()
    parser.add_argument("pdf", help="Input PDF")
    parser.add_argument("md", help="Output Markdown file")
    args = parser.parse_args()

    pdf_to_markdown(args.pdf, args.md)

