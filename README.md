# CT-imaging-deidentification
ProTECT III master imaging dataset deidentification

M. Lunney 

  21AUG2015 -original
  
  19JUN2018 -edited for GitHub

All images deidentified using [RSNA Clinical Trials Processor](https://www.rsna.org/ctp.aspx) (many thanks to John Perry for all of his support of this project).


All `PatientID (0010,0020)` and `InstitutionName (0008,0080)` tags changed to correspond with ProTECT Public-Use Dataset (PUDs). FITBIR GUID used as `PatientName (0010,0010)`.

`PatientsSex (0010,0040)` and `PatientsAge (0010,1010)` are true. `AdditionalPatientHistory (0010,21b0)` is true mechanism of injury.

Time/date of scans changed relative to a time of injury of 0000 hrs on 01JAN2000. For example, a scan with the time/date of 0600 on 05JAN2000 was taken 102 hours post-injury. Absolute time from injury listed in `StudyComments (0032,4000)` tag.

File tree folder structure is: 

    ID_number
      Date  
        Series
