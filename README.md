# learning-azure

Azure Developer Workshop (Storage, Cognitive, ML, Stream Analytics, Containers, and Docker)
https://mva.microsoft.com/en-US/training-courses/azure-developer-workshop-storage-cognitive-ml-stream-analytics-containers-and-docker-17033?l=qaxmpcPND_5706218965

# 01 - Intro to the Microsoft Cloud

[img01]

# 02 - Creating an Azure Subscription

Get a free account/trial - http://azure.microsoft.com
	• $200 Azure credit
Login - https://portal.azure.com


# 03 - Azure Storage and Cognitive Services

Azure Storage Types
[img02]

(Focus on just Blobs for this course)
[img03]

Replication Options (More details: https://docs.microsoft.com/en-us/azure/storage/)storage-redundancy
LRS	Locally Redundant Storage - Replicated three times within a single facility in a single region
ZRS	Zone-Redundant Storage - Replicated three times across two to three facilities, either within a single region or across two regions
GRS	Geo-Redundant Storage - Replicated three times within the primary region, and is also replicated three times in a secondary region hundreds of miles away from the primary region
RA-GRS	Read Access Geo-Redundant Storage - Replicates your data to a secondary geographic location, and also provides read access to your data in the secondary location

Storage Containers Access
Private	Can't be read or enumerated anonymously
Public Container	Can be read and enumerated anonymously
Public Blob	Blobs can be read, but not enumerated

Storage Blob Types
Block	195 GB	General-purpose streaming and storage
Append	195 GB	Optimized for append operations
Page	1 TB	VHDs only; optimized for random access

Storage Keys
	• Can access everything you can, use for code-to-code, NOT to another person
	• Should be "rolled" periodically for security
	• Can be used to generate shared-access signatures (SAS) for secure and restricted access
		○ Can specify expiration
		[img04]

Azure Storage Tools
	• Microsoft Azure Storage Explorer
		○ http://storageexplorer.com/
	• Azure Command-Line Interface
		○ https://azure.github.io/projects/clis/
