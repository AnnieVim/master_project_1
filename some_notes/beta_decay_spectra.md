# $\beta$-decay spectra calculation

&emsp;&emsp;
Under Fermi goldern rule, we could acquire the transition probability between two quantum states. And for $\beta$-decay (<font color=gree>hint: we just talk about $\beta ^-$ decay here</font>), the probability of a $\beta$ particle with momentum arranging from *p* to *p + dp* emitted from a nucleus $\lambda$ is

$$\lambda=I(p)dp=\frac{2\pi}{\hbar}|\langle \Psi_f|H|\Psi_i \rangle|^2\rho(E_f) \tag{1},$$

in which, *$H$* is the weak interaction operator, $\Psi_f$ is the final (<font color = gree>i.e. post decay</font>) wave funciton, $\Psi_i$ is the initial (<font color=gree>i.e. before decay</font>) wave function, respectively. And $\rho(E_f)=dn/dE_f$ is the energy density of the post-decay system.

&emsp;&emsp;
We calculate the fomula beyond from two separate parts, $\rho(E_f)$ and $|\langle \Psi_f|H|\Psi_i \rangle|^2$

---
&emsp;&emsp;
For the first part $\rho(E_f)$,

$$dn = \prod dn_{\beta}dn_{\nu}dn_{d} \tag{2},$$

in which, $dn_{\beta}$, $dn_{\nu}$ and $dn_d$ indicate the number of the $\beta$ paricle, $\bar\nu_e$ and the daughter nucleus state, respectively. For a specific decay, $dn_d$ equals to 1. And for $\beta$ particle and anti-neutrino emitted arranging from $p_{\beta}$ to $p_{\beta}+dp_{\beta}$ and $p_{\nu}$ to $p_{\nu}+dp_{\nu}$ , the number of state in phase space could be given as

$$dn_{\beta}=\frac{V \times 4\pi p_{\beta}^2 dp_{\beta}}{(2\pi\hbar)^3},\ \ dn_{\nu}=\frac{V \times 4\pi p_{\nu}^2 dp_{\nu}}{(2\pi\hbar)^3} \tag{3},$$

so that equation (2) could be written as 

$$dn = \frac{V^2 p_{\beta}^2 p_{\nu}^2 dp_{\beta} dp_{\nu}}{4\pi^4\hbar^6}. \tag{4}$$

&emsp;&emsp;
After decay, the released energy is shared by $\beta$ particle, anti-neutrino and the daughter nucleus, respectively, and $E_f=E_{\beta}+E_{\nu}+E_{d}$ (<font color=gree>actually $E_f$ equals decay energy $Q_i$</font>), generally speaking, the mass of daugher nucleus is much larger than the other two particles, so that its kinetic energy $E_{d}$ is small, and we could move it away, and $E_f=E_{\beta}+E_{\nu}$, and $dE_f=dE_{\nu}$.

&emsp;&emsp;
Through special relativity (S.R.), the particle energy $E=\sqrt{m^2c^4+p^2c^2}$, while the mass of anti-neutrino is small, and we could ignore the first term, and $E_{\nu}=p_{\nu}c$, as a result $dE_{\nu}=cdp_{\nu}$. On the other hand, $E_f=E_{\beta}+p_{\nu}c$, as a result $p_{\nu}=(E_f-E_{\beta})/c$. On the basis of what we draw beyond, $\rho(E_f)$ could be written as 

$$\rho(E_f)=\frac{dn}{dE_f}=\frac{(E_f-E_{\beta})^2 p_{\beta}^2 V^2}{4\pi^4\hbar^6c^3}dp_{\beta} \tag{5}.$$

---
&emsp;&emsp;
For the second part $|V_{fi}|^2=|\langle \Psi_f|H|\Psi_i \rangle|^2$, the wave function $\Psi_f$ and $\Psi_i$ could be written as $\Psi_f=\psi_d\psi_{\beta}\psi_{\nu}$ and $\Psi_i=\psi_i$, respectively. <font color=gree>To simplify calculation, first, we ignore the coulomb interaction temporarily,</font> so that $\psi_{\beta}=e^{i\vec k_{\beta}\cdot \vec r}/\sqrt{V}, \psi_{\nu}=e^{i\vec k_{\nu}\cdot \vec r}/\sqrt{V}$. <font color=gree>And then we draw weak interaction opetator $H$ as a constant $G_F$.</font> Then we could know 

$$
\begin{aligned}
|\langle \Psi_f|H|\Psi_i \rangle|^2 &= |\int_V \Psi_f^* H \Psi_i |^2 
\\ &=  \frac{G_F^2}{V^2}|\int \psi_f^* \psi_i \cdot exp[-i(\vec k_{\beta}+ \vec k_{\nu})\cdot \vec r]dV|^2
\\ &= \frac{G_F^2}{V^2}|M_{fi}|^2,
\end{aligned}
\tag{6}
$$

in which, we call $|M_{fi}|$ the transition matrix element.

---
&emsp;&emsp;
We put eq.(5) and eq.(6) into eq.(1), and we get

$$
\lambda=\frac{G_F^2 |M_{fi}|^2}{2\pi^3 c^3 \hbar^7}(E_f-E_{\beta})^2 p_{\beta}^2 dp_{\beta}.
\tag{7}
$$

&emsp;&emsp;
At the begining, we ignore coulomb interaction, now we intoduce coulomb correlation factor (also named as $Fermi \ function$) $F(Z_{d}, E_{\beta})$ which is a complicated function  to modify such simplification, and eq.(7) turns to

$$
\begin{aligned}
\lambda =I(p_{\beta})dp_{\beta}&=\frac{G_F^2 |M_{fi}|^2}{2\pi^3 c^3 \hbar^7}F(Z_{d}, E_{\beta})(E_f-E_{\beta})^2 p_{\beta}^2 dp_{\beta}
\\ &=\frac{G_F^2 |M_{fi}|^2}{2\pi^3 c^3 \hbar^7}F(Z_{d}, E_{\beta})(E_f-E_{\beta})^2 (\frac{E_{\beta}^2}{c^2}+m_{\beta}^2 c^2) dp_{\beta}.
\end{aligned}
\tag{8}
$$

---
## References
[1] 卢希庭[M].北京:原子能出版社, 2010:140-146

[2] [H. Behrens and J. Janecke, ¨ Landoldt-Bornstein Tables, Gruppe ¨I (Springer, Berlin, 1969), Vol. 4.](https://materials.springer.com/bp/docs/978-3-540-36068-1)

[3] [J. C. Hardy and I. S. Towner, Phys. Rev. C 79, 055502 (2009)](https://journals.aps.org/prc/abstract/10.1103/PhysRevC.79.055502)







