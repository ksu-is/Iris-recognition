This is my road map file.
Found this repository https://github.com/OmarMedhat22/Iris-Recognition-CASIA-Iris-Thousand, had trouble running but a very short code I can use for my project
# Code to read Iris Data
class IrisDataset(Dataset):
    def __init__(self, csv_file, root_dir, transform=None):
        self.annotations = pd.read_csv(csv_file)
        self.root_dir = root_dir
        self.transform = transform
