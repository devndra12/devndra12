- 👋 Hi, I’m @devndra12
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
devndra12/devndra12 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
# import module
import os

# assign size
size = 0

# assign folder path
Folderpath = 'C:/Users/Geetansh Sahni/Documents/R'

# get size
for path, dirs, files in os.walk(Folderpath):
	for f in files:
		fp = os.path.join(path, f)
		size += os.path.getsize(fp)

# display size
print("Folder size: " + str(size))
