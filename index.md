<button id="darkModeToggle" aria-label="Toggle dark mode">
  <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
    <path d="M21 12.79A9 9 0 1 1 11.21 3 7 7 0 0 0 21 12.79z"></path>
  </svg>
</button>

## About Me
I am a Ph.D. student in the Department of Computer Science at Tulane University. Deep Reinforcement Learning, Causal Inference, and Bayesian Networks are my interests. I completed my Master's degree in Mechanical Engineering from Iowa State University in 2019. My Master's research was on mechano-chemical milling techniques.

## Publications and Preprints

- Ghanbari, Ali, et al. "Mutation-based Fault Localization of Deep Neural Networks." 2023 38th IEEE/ACM International Conference on Automated Software Engineering (ASE). IEEE, 2023. **[Distinguished Paper Award]** 

- Thomas, Deepak George, Tichakorn Wongpiromsarn, and Ali Jannesari. "Temporal shift reinforcement learning." Proceedings of the 2nd European Workshop on Machine Learning and Systems. 2022.

- Thomas, Deepak-George, Daniil Olshanskyi, Karter Krueger, and Ali Jannesari. "Interpretable UAV Collision Avoidance using Deep Reinforcement Learning." arXiv preprint arXiv:2105.12254 (2021). [[Preprint]](https://github.com/Deepakgthomas/deepakgthomas.github.io/files/9294702/2105.12254.pdf)
  
  
- Thomas, D.G., De-Alwis, S., Gupta, S., Pecharsky, V.K., Mendivelso-Perez, D., Montazami, R., Smith, E.A. and Hashemi, N.N., 2021. Protein-assisted scalable mechanochemical exfoliation of few-layer biocompatible graphene nanosheets. Royal Society open science, 8(3), p.200911.   
 
- Shihab, Syed Arbab Mohd, Caleb Logemann, Deepak-George Thomas, and Peng Wei. "Autonomous airline revenue management: A deep reinforcement learning approach to seat inventory control and overbooking." arXiv preprint arXiv:1902.06824 (2019).

- Thomas, Deepak-George. "Exfoliation of scalable few layer biocompatible graphene nanosheets using a protein-assisted mechano-chemical technique." Master's dissertation, Iowa State University, 2019. [[Thesis]](https://github.com/Deepakgthomas/deepakgthomas.github.io/files/9294745/Thomas_iastate_0097M_17985.pdf) 

- Thomas, Deepak-George, Emrah Kavak, Niloofar Hashemi, Reza Montazami, and Nicole N. Hashemi. "Synthesis of graphene nanosheets through spontaneous sodiation process." C 4, no. 3 (2018): 42.

- McNamara, Marilyn C., Farrokh Sharifi, Alex H. Wrede, Daniel F. Kimlinger, Deepak‐George Thomas, Jonathan B. Vander Wiel, Yuanfen Chen, Reza Montazami, and Nicole N. Hashemi. "Microfibers as physiologically relevant platforms for creation of 3D cell cultures." Macromolecular bioscience 17, no. 12 (2017): 1700279.

- Tan, Russell Kai Liang, Sean P. Reeves, Niloofar Hashemi, Deepak George Thomas, Emrah Kavak, Reza Montazami, and Nicole N. Hashemi. "Graphene as a flexible electrode: review of fabrication approaches." Journal of Materials Chemistry A 5, no. 34 (2017): 17777-17803. 

## Service

- Technical Program Committee Member: EuroMLSys @ EuroSys 2024
- Technical Program Committee Member: EuroMLSys @ EuroSys 2023
- Reviewer for Transactions on Emerging Topics in Computational Intelligence

## Work Experience

- **Fellow**<br>
  *Data Science for the Public Good (DSPG) Summer Program*, Ames, Iowa, May 2020 – August 2020 <br><br>
- **Integrated Solutions Engineering Co-op, Research and Development**<br>
  *Danfoss*, Ames, Iowa, Jan 2019 – Aug 2019 <br><br>
- **Design Engineering Co-op, Global Product Organization**<br>
  *Whirlpool Corporation*, Amana, Iowa, Jan 2018 – July 2018<br><br>
- **Research and Development Intern**<br>
  *ArcelorMittal USA - Research Facility*, East Chicago, Indiana, May 2017 – Aug 2017

<style>
body {
    transition: background-color 0.3s, color 0.3s;
}
.dark-mode {
    background-color: #1a1a1a;
    color: #ffffff;
}
.dark-mode a {
    color: #bb86fc;
}
#darkModeToggle {
    position: fixed;
    top: 10px;
    right: 10px;
    width: 40px;
    height: 40px;
    border-radius: 50%;
    background-color: transparent;
    border: none;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
    z-index: 1000;
}
#darkModeToggle svg {
    width: 24px;
    height: 24px;
    color: #333;
}
.dark-mode #darkModeToggle svg {
    color: #fff;
}
</style>

<script>
function toggleDarkMode() {
    document.body.classList.toggle('dark-mode');
    localStorage.setItem('darkMode', document.body.classList.contains('dark-mode'));
    updateIcon();
}

function updateIcon() {
    const isDarkMode = document.body.classList.contains('dark-mode');
    const icon = document.querySelector('#darkModeToggle svg');
    if (isDarkMode) {
        icon.innerHTML = '<circle cx="12" cy="12" r="5"></circle><line x1="12" y1="1" x2="12" y2="3"></line><line x1="12" y1="21" x2="12" y2="23"></line><line x1="4.22" y1="4.22" x2="5.64" y2="5.64"></line><line x1="18.36" y1="18.36" x2="19.78" y2="19.78"></line><line x1="1" y1="12" x2="3" y2="12"></line><line x1="21" y1="12" x2="23" y2="12"></line><line x1="4.22" y1="19.78" x2="5.64" y2="18.36"></line><line x1="18.36" y1="5.64" x2="19.78" y2="4.22"></line>';
    } else {
        icon.innerHTML = '<path d="M21 12.79A9 9 0 1 1 11.21 3 7 7 0 0 0 21 12.79z"></path>';
    }
}

document.getElementById('darkModeToggle').addEventListener('click', toggleDarkMode);

// Check for saved dark mode preference
if (localStorage.getItem('darkMode') === 'true') {
    document.body.classList.add('dark-mode');
}
updateIcon();
</script>
