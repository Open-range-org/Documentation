# csv-grape

A library that handles csv files and its metadata for js or typescript projects.

## Installation

```bash
npm install csv-grape

```




## Initiate the service

```bash
import { CsvGrape } from 'csv-grape';

```

## Get all csv content

```bash

    CsvGrape.getCsvData(event).then((_response)=>{
      this.data=_response;
      
    },(reject)=>{
      console.log(reject);
    });

```
##  Get csv file metadata

```bash
//Here we can get _response from getCsvData(event)
this.csvMetaData=  JSON.stringify(CsvGrape.getMetaData(_response.Data,_response.Headers));

```
##  Get csv content with metadata

```bash

CsvGrape.getCsvWithMetaData(event).then((_response)=>{
      this.csvJsonAndMetaData=_response;
    },(reject)=>{
      console.log(reject);
    });

```

