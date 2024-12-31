# Nexus File Writer for Neutron Data 📊🔬  

This repository provides a tool for writing **NeXus** files in the HDF5 format, adhering to neutron data standards. It includes examples and supports writing NeXus files using SNS input information for neutron experiments.

---

## Features ✨  

- **NeXus File Creation**: Write NeXus-compliant HDF5 files for neutron experiment data.  
- **Standardized Format**: Ensures compatibility with neutron data standards.  
- **Input Example**: Includes an example file for SNS input information.  

---

## Prerequisites 🛠️  

- Python 3.8+  
- Required Python libraries:
  - `h5py`  
  - `numpy`  

Install dependencies:  
pip install h5py numpy  

---

## Installation  

1. Clone the repository:  
git clone https://github.com/your-username/nexus-file-writer.git  
cd nexus-file-writer  

2. Install dependencies:  
pip install -r requirements.txt  

---

## Usage 🔧  

1. **Write a NeXus File**:  
Run the script to create a NeXus file:  
python write_nexus.py --input sns_input.json --output output_file.nxs  

2. **Modify Input Information**:  
Edit `sns_input.json` to match your neutron experiment details, such as:  
- Instrument name  
- Sample metadata  
- Detector data  

---

## File Structure 📂  

- `write_nexus.py`: Main script for writing NeXus files.  
- `sns_input.json`: Example input file for SNS neutron experiment metadata.  
- `README.md`: Documentation for the repository.  

---

## Example Input (`sns_input.json`)  

```json
{
  "instrument": "SNS",
  "sample": {
    "name": "Test Sample",
    "temperature": 300
  },
  "detectors": {
    "counts": [100, 200, 150],
    "time_of_flight": [0.1, 0.2, 0.3]
  }
}
