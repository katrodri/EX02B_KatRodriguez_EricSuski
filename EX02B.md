# Vet Office List Normalization
## Step 1: Identify all candidate keys of the relation
1. PetName
2. OwnerPhone
3. OwnerEmail
## Step 2: Identify functional dependencies
1. PetName-(PetID, PetBreed, PetDOB)
2. OwnerEmail-(OwnerFirstName, OwnerLastName, OwnerPhone)
3. OwnerPhone-(OwnerLastName,OwnerFirstName,OwnerEmail)
4. Service -> Charge
## Step 3: Make Determinants Candidate Keys
1. PetInfo (**PetName**, PetType, PetBreed, PetDOB, *OwnerEmail*)
2. OwnerInfo (**OwnerEmail**, OwnerLastName, OwnerFirstName, OwnerPhone)
3. ServiceInfo (**Service**, Charge, Date, PetName, *OwnerEmail*)
