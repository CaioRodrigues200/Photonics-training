# Microring resonator

A microring resonator is a looping photo-conductor device that utilizes resonnace phenomenon to filter or deliver energy from different silicon buses. There are originally two types of microring resonator layouts: All-pass and Add-drop.

## All-pass ring resonator
All-pass ring resonator is its simplest form, consisting by feeding one output of a directional coupler back into its input, while the other waveguide of the pair stays unchanged, often called bus waveguide.

![All Pass Scheme](Media/All-Pass-Scheme.png)

$r$ is the [self-coupling](https://opg.optica.org/oe/fulltext.cfm?uri=oe-17-21-18971&id=186494#e03) ratio and $k$ the [cross-coupling](https://opg.optica.org/oe/fulltext.cfm?uri=oe-17-21-18971&id=186494#e03) ratio.
Assuming no reflections back into the bus waveguide, the following can be stated:

$$ r = \frac{|t_{c}'|}{\alpha_{c}'} $$  

$$ k = \frac{|k_{c}'|}{\alpha_{c}'} $$

$$ (\alpha_{c}')^2 = |t_{c}'|^2 + |k_{c}'|^2 $$ 

Where $t_{c}'$ and $k_{c}'$ are the self-coupling and cross-coupling coefficients at the ring respectively. $\alpha_{c}'$ is the loss function at the ring, so that $\alpha_{c}' = 1$ means no coupling loss and $\alpha_{c}' = 0$ full coupling loss. Note that $r^2 + k^2 = 1$.

Knowing $t_{r}'$ as the ring back-coupling coefficient, it can be defined the single-pass amplitude transmisstion, including both propagation loss in the ring and loss in the couplers:

$$ a = |t_{r}'|\alpha_{c}' $$  

It relates to the power attenuation coefficient $\alpha$ [1/cm] as $a^{2} = e^{-\alpha L}$, with $L$ being the round trip length.

![DC Transmission Coefficients](Media/DCTransmissionCoefs.png) ![RR Transmission Coefficients](Media/RRTransmissionCoefs.png)

Assuming no reflections back into the bus waveguide, can be stated that the ratio between the transmited and incident field on it is:

![Transmited Field Ratio](Media/TransmitedFieldRatio.png) (eq.1)

where $\phi = \beta L$ is the single-pass phase shift with $\beta$ being the [Propagation constant](https://www.rp-photonics.com/propagation_constant.html).

By squaring the (eq.1) it can be obtained the intensity transmission:

![Transmission Ratio](Media/TransmissionRatio.png) (eq.2)

Can be observed that the ring will be on resonance when the single-pass phase shift $\phi$ is a multiple of 2$\pi$, or when the wavelength of the light fits a whole number of times inside the [Optical length](https://www.microscopyu.com/tutorials/specimen-optical-path-length-variations) of the ring:

![Transmission Ratio](Media/WavelengthFit.png) (eq.3)

The effective phase shift $\varphi$ induced by the ring resonator can be calculated manipulating (eq.1):

![Transmission Ratio](Media/PhaseShift.png) (eq.4)

