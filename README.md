# UNet-Domain-Generalization

Downloaded the Zip file from http://www.midaslab.org/autoPET/data/nifti.zip using Sagemaker Jupyter Notebook instance. and extract them to s3 location 

Clinical Data (csv)
https://wiki.cancerimagingarchive.net/download/attachments/93258287/Clinical%20Metadata%20FDG%20PET_CT%20Lesions.csv?api=v2

file strcuture 

|--- Patient 1
     |--- Study 1
          |--- SUV.nii.gz    (PET image in SUV)
          |--- CTres.nii.gz  (CT image resampled to PET)
          |--- CT.nii.gz     (Original CT image)
          |--- SEG.nii.gz    (Manual annotations of tumor lesions)
          |--- PET.nii.gz    (Original PET image as actictivity counts)
     |--- Study 2            (Potential 2nd visit of same patient)
          |--- ...
|--- Patient 2
     |--- ...
	 

