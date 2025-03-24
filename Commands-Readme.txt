* to execute
  mvn clean install exec:java -Dexec.mainClass="mainapp.MyApp" -DskipTests=true

* to run test cases
  mvn test

--------------------------------------------------------------------------------
echo "This is the initial content." > index.txt
echo "This is the about page content." > about.txt
git add index.txt about.txt
git commit -m "Initial commit: Add index and about text files"

echo "Updated content for the homepage." > index.txt
echo "Updated about page content." > about.txt
git add index.txt about.txt
git commit -m "Update content in index.txt and about.txt"

git reset --soft <last hash>

git reset --hard <very first commit hash>

echo "Corrected content for the homepage." > index.txt
echo "Corrected about page content." > about.txt
git add index.txt about.txt
git commit -m "Corrected content in index.txt and about.txt"
