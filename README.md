- 👋 Hi, I’m @Matias-Lima
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Matias-Lima/Matias-Lima is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

const { Contributions } = require('contributions')

const contributions = await Contributions.forUser('ethomson');
const days = contributions.getDays();

for (let day of days) {
    console.log(`${day.getDate()}: ${day.getIntensity()}`);
}
