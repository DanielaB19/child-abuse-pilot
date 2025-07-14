# experiment-s1-child-abuse-neglect

# ARTIFICIAL INTELLIGENCE IN CHILD ABUSE AND NEGLECT

This repository hosts the project developed for the Master's Thesis in Ethics in Artificial Intelligence, for the Master's program in Artificial Intelligence at the University of Bologna, during the 2024–2025 academic year.

## Abstract

According to the latest national investigation carried out by the Guarantor Authority for Childhood and Adolescence (Autorità Garante per l’Infanzia e l’Adolescenza), the cases of maltreatment of children and adolescents have increased by 58% in five years. The need to have an effective tool and system for the early identification of abuse and maltreatment led Sant’Orsola’s doctors to propose a collaboration with the Artificial Intelligence department of the University of Bologna to study the possibility of including AI technology to tackle this problem.

In this thesis, after researching known solutions, we performed rule-extraction on the professional manuals provided by the doctors. The manuals describe the symptoms that can be found in the patients at risk, along with the behavior that the doctor should have during the patient–doctor interaction and the steps that the doctor and the hospital should follow.

After extracting the rules, we analyzed, restructured, and summarized them into questions. We studied two important instruments, ESCAPE and SCAN, that were born with the same aim as our project and compared our questions with the questionnaires described in these two studies.

This project resulted in the creation of a 5-item checklist that is designed to assist the medical professional that encounters an at-risk patient to determine whether the child could be a victim of abuse or maltreatment.

In the future, the aim is to incorporate this tool as a standard step during any clinical consultation of a minor, in order to drastically reduce the cases of maltreatment and abuse of children and adolescents in Italy.

This project contains the code used to extract the rules from the provided manuals and test our proposed checklist on the clinical cases contained in the provided dataset.

## Structure

- `child_abuse_neglect_rule_extraction.ipynb`: Colab notebook with the rule extraction code and the code to test the checklist
- `requirements.txt`: List of dependencies

## Usage

The notebook `child_abuse_neglect_rule_extraction.ipynb` runs a pipeline that:
1. Extracts the rules from pdf manuals using gpt-4 and writes them in one docx document for each manual
2. Fills in a questionnaire for each medical case in the inputed database
3. Prints the confusion matrix of the results

## Note

The code is tailored to fit the database and the manuals that we used on the project. Since both the database and the manual are not public, they are not included in this project.

The code is set up to connect to google drive to access the data.

 

## Disclaimer

This project is for research and ethical evaluation only. Not intended for clinical use.
