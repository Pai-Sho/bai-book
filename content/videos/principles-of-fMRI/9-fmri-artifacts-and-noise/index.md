# Video

<iframe width="560" height="315" src="https://www.youtube.com/embed/7Kk_RsGycHs" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

# Questions

## Drift

![drift](drift.png)

Q. Why is it not possible to detect the signal in this example?

A. Because the magnitude of the drift is much higher than the signal, and there is only one period of signal which is not enough data to separate it from the drift.

## Aliasing

![hrf](hrf.png)

Q. Given a TR of 2000ms, is it possible to avoid aliasing when sampling from the HRF shown above? Why or why not?

A. The signal shown in the HRF is not periodic, so aliasing doesn't really apply in this case. Assuming the signal repeats every 5 seconds, it would be possible to avoid aliasing since that corresponds to a 0.5Hz sampling frequency, which is more than double the signal frequency of 0.2Hz, and therefore is greater than the Nyquist frequency.

Q. What could possibly be the largest TR while avoiding aliasing? Why?

A. 2500ms, or 2.5 seconds with the assumptions made above.

## Noise Map

![noise map](noise-map.png)

Q. If the noise were uniform across the entire brain, what would the spatial map look like instead?

A. The map would be a uniform color

Q. If noise were higher closer to the center of the brain, what would the spatial map look like instead?

A. It would be brighter towards the center and dimmer further away
