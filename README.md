# autocorrelation_1

For an ARMA(1,2) process, the extended Yule-Walker equations are used to relate the autocorrelations of the process (\(\rho_k\)) with the model parameters. The equations for the first two lags are:

**For lag 1:**
\begin{equation*}
    \rho_1 = \phi \rho_0 + \theta_1 \rho_1 \phi + \theta_2 \rho_2 \phi
\end{equation*}
Where \(\rho_0 = 1\) (autocorrelation at time 0), \(\phi = 0.5\), \(\theta_1 = -0.3\) and \(\theta_2 = -0.28\).

**For lag 2:**
\begin{equation*}
    \rho_2 = \phi \rho_1 + \theta_1 \rho_1 + \theta_2
\end{equation*}
Here there is no term for \(\rho_0\) since the lag is 2.

We solve these two equations simultaneously for \(\rho_1\) and \(\rho_2\). Substituting the values of \(\phi\), \(\theta_1\), and \(\theta_2\) into the equations, we get:

**For lag 1:**
\begin{equation*}
    \rho_1 = 0.5 + (-0.3) \times 0.5 \times \rho_1 + (-0.28) \times 0.5 \times \rho_2
\end{equation*}

**For lag 2:**
\begin{equation*}
    \rho_2 = 0.5 \times \rho_1 - 0.3 \times \rho_1 - 0.28
\end{equation*}

Then we solve these equations simultaneously to find the values of \(\rho_1\) and \(\rho_2\).

After solving the equations, we find that:
\begin{align*}
    \rho_1 &= 0.4577 \\
    \rho_2 &= -0.1885
\end{align*}
These values represent the autocorrelation of the process at lags 1 and 2, respectively.
