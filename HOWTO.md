`start_step` in `Color Adjust` node **does not mean** "`start_at_step` of KSampler" but **N steps FROM the BEGINNING of SAMPLING**,
if you set it to `5` while my 2nd KSampler in multi-stage sampling setup was `start_at_step=5` `end_at_step=10`,
it never color corrects.

Set it to `0` and then it should work, **from step `5`**.
