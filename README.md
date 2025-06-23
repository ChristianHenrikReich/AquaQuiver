# AquaQuiver
This is a pico-example of a Apache Arrow based meta-data driven lakehouse for Microsoft Fabric. For a full scale solution, I recommend twoday's AquaVilla best practices.

If wanting an Apache Spark based version of a meta-data driven lakehouse for Microsoft Fabric, there is also [AquaShack](https://github.com/ChristianHenrikReich/AquaShack)

## Notes

Currently, due to Microsoft Fabric, it have to run on PySpark compute instead of a Python Notebook compute.

## Installation 

/Setup.ipynb holds all to get started. It is one script, to setup the full example.

## Documentation

AquaQuiver is traditionel medallion architecture, due to history the Bronze, Silver and Gold layers are named Landing, Base and Curated.

When installed, the notebook 1_AquaShack_Landing_To_Base will move example data from Landing to Base. 
The notebook 2_AquaShack_Base_To_Curated will move data from Base to Curated.

![image](https://github.com/user-attachments/assets/470adae5-d49d-4ffd-a23e-49cf29e1f1ec)

### Project layout

<img width="1794" alt="image" src="https://github.com/user-attachments/assets/23e4484a-ed49-4e07-a944-e8c59a0ae7ec" />


## Articles

[Delta and Parquet: Integer, GUID/UUID or SHA256 as ID?](https://medium.com/@christianhenrikreich/delta-and-parquet-integer-guid-uuid-or-sha256-as-id-67ba15b4437f)

[Spark SQL: Why the choice of language doesn’t impact performance](https://medium.com/@christianhenrikreich/spark-sql-why-the-choice-of-language-doesnt-impact-performance-747ff3f854ae)

[Data Architecture: Data capture time and event time in medallion architecture](https://medium.com/@christianhenrikreich/data-architecture-data-capture-time-and-event-time-in-medallion-architecture-dceb93980e0a)

[Microsoft Fabric: Building Pseudo Identity Columns Without monotonically_increasing_id() in Spark](https://medium.com/@christianhenrikreich/microsoft-fabric-building-pseudo-identity-columns-without-monotonically-increasing-id-in-spark-09b1efb577d1)

[Lakehousing: Removing one of the biggest performance killers in Silver-to-Gold processing](https://medium.com/@christianhenrikreich/lakehousing-removing-one-of-the-biggest-performance-killers-in-bronze-to-silver-processing-8ed4ce372de6)
