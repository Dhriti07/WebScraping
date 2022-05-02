# Web Scraping Project:

## Aim:
URL: https://marketplace.akc.org/puppies

- For each listing in the url extract the following info from the “about the breeder” section:
   1. Breeds
   2. Kennel Name
   3. Breeder Name
   4. Website 
   5. Location 
   6. Phone number 
 
- If there are multiple breeds seperated by a comma, then there need to be seperate recordings for each breed 
- If the wesbite is missing, add a website using the following method :
  - If there is a ?, stop just before: https://marketplace.akc.org/breeder/weatherby-goldens?source_breed=golden- retriever → https://marketplace.akc.org/breeder/weatherby-goldens
  - If there is no ?, stop after the second / after breeder: https://marketplace.akc.org/breeder/kimberly-fritzler-43217/greyhound/321167 → https://marketplace.akc.org/breeder/kimberly-fritzler-43217/
  
- Remove Duplicates if any from the list 

- Store the extracted data in a txt file organized by
  - breed in alphabetical order
  - Within each breed, order by state in alphabetical order
  - Withing each state, recordings must be in alphabetical order by kennel name
