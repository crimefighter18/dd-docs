# GitLab

### Steps to Integrate with GitLab

1.  Log in to DevDynamics ([devdynamics.ai](https://devdynamics.ai/))

    <figure><img src="https://lh5.googleusercontent.com/6w20F89Of7kNQXM6X2te6Ne87CgxGwcWKX2OJCxQJ2Hc-lFRExGjvDjsj33cefVpaR8_uT0eqPvn8ZgeuKMOVDWSekWo-VCwWo43R1RiO8_-qgZh_Lv2kjZCvfBy7fk66sPJxnYXwZL1bD03yDY3wtg" alt=""><figcaption></figcaption></figure>
2.  Go to Settings --> Integrations.

    <figure><img src="https://lh4.googleusercontent.com/0ZZ0mLS5wu6anN6PHtYlvLyciZ4l76lHnMgkDIE77RxrQM0pcIQOTbWIxeKrYebAtuPN_0Pg17j0SRaf3x32zSg5gEU-TdpFL75O7SonH10_Xxxn6Y_NK6dfgfUGmL3YCEdsSXfSmAIR4NaHSx1eDZ0" alt=""><figcaption></figcaption></figure>
3.  Click on Integrate under GitLab

    <figure><img src="https://lh3.googleusercontent.com/Sivel7WQwhinTR7aV0NL2lu1mRV5yZBoTqTUhdq0YjG_bkPq5PXW1b9rjEOXiPjGEXHdufjF-_3PSmVPJJDKCSN2Uky_L7zy6gNhNKfxRyDE4bgbkjeR1CDYaRA24d-nURn3tL9u51SFxXdX3WKd0nE" alt=""><figcaption></figcaption></figure>
4.  Click on Integrate GitLab

    <figure><img src="https://lh4.googleusercontent.com/XKK9oOFyTvKcowr4GlzAGagsb2BE09Ha35oCmXYvLtKvOy7kPykNqkhjYAvPJEGPOYYSA1-7zr0aj9PZ638phQImj0CMoPJ_t0RZQl9tnFPH6LvduPlV5YpxETsk8l0pVu78QxkRZkfPvffaop6REL0" alt=""><figcaption></figcaption></figure>
5.  Sign in to [GitLab](https://about.gitlab.com/)

    <figure><img src="https://lh5.googleusercontent.com/NM4EvvfMr9mZoH7uBlFI3loLD76OpzmRohjOcEGgbvFXKjFJ2XbILspOdVGdm7qYbTa7LU3ZV6Qjqtoz9hR_M3Tp2AOj9TkWNP6CdFcUKa9g_ZhiaTr0NBOFflxa3kmg1r17WmEmAD2bTo3Y6vKPkBs" alt=""><figcaption></figcaption></figure>

#### To generate API Token

{% hint style="info" %}
Make sure that you have a maintainer role or above to perform this action.
{% endhint %}

6.  Click on the Profile icon and go to Preferences. This will redirect you to the User Settings page.

    <figure><img src="https://lh3.googleusercontent.com/DbgI2XTEleoNsqK3ZZ_yaKqf7yDkSqFk9RyL3V6I-ifFmJ7r27JUPke9mqXY81mbFHXkYte_kNCXqju_gOhiE-nC-Mh5xeZcX0Vczsw7TiDVrtGJ-mR22a8f5dylYpZTYptJMK__IryiC6FLLfKomyU" alt=""><figcaption></figcaption></figure>
7.  Under User Settings, click on Access Tokens. Enter a name for the access token. Keep the expiration date empty.

    <figure><img src="https://lh4.googleusercontent.com/2X_FSUlAEDu6HffsUaKvXybTlLxYFxgD_6sk58GmrEitQPd8uoWgOrOE-pIGj2LDTfOl8diCdcoZ-DN1KQzRdTjRc53nFZrI3wYEdqZCSyKShHzPRC04FmTagVIImWX8gfJk6uzKuE2hoMgwjQA1lkc" alt=""><figcaption></figcaption></figure>
8.  Select the following scopes and click on Create personal access token.

    1. api
    2. read\_api
    3. read\_user
    4. read\_repository

    <figure><img src="https://lh3.googleusercontent.com/-V1VWoVY16wkiOFTofs3aiWRxKN6AX1Jo7Qdw4Jm9pVHNRcVKlcoTjY60mgujZ-7EhKL3rIcci4SBG78VtRXOpdrkg9fPmYw618VD2xyIBnUSD3DSCy0pt6PY2_iOjdRjG125DiqFcCdfrKaWSPouuY" alt=""><figcaption></figcaption></figure>
9.  Your new personal access token will be generated. Save the token.\
    _NOTE: This token will be visible only once._

    <figure><img src="https://lh4.googleusercontent.com/HJG2YMxtUiG70lQIIDGRw8eBWy_ui9Zzyn8hieoBJ8ZjJ57wcX-mkZSu1ICrl13E8mpgIB1HWLMMAvoZoxphnwIVnIjJyn0D5ojvUlXaTZPrTrDi-WN3D93F-iI2u25-WEt75z647xdJ2Nlfcn3hCjA" alt=""><figcaption></figcaption></figure>

#### Steps to derive GitLab base URL:

10. Go to the GitLab home page (gitlab.com) and click the Profile icon.\
    \
    Click on your Profile Name

    <figure><img src="https://lh3.googleusercontent.com/3dEAxxZJNjWXl8Akc0476liN6T52GKS_DqweX5_38sM8GFpg2gMocyZAge1soKhwzemF5sPF3HoRuLmt93ZiPt5eg8POoJUrBMrJeZuAevDEER2lHBT9etUSa_v6NhPSJHrP8avIw8Rfyog9_iGyf7Q" alt=""><figcaption></figcaption></figure>
11. You will be redirected to your Profile page. The URL of this page is your required Base URL.

    <figure><img src="https://lh4.googleusercontent.com/T3D3p_BjNb6pHs0Fwx_cW5ydwBYYsAqfzDACodouQ5BguL3PrfMecAG36Qc242TjiDi1lZpF6H93wlg59ZdFZz-ueWe4q_cu6O6u29DzMeugY-ZMOJhPHbNPU0kROxWnXUZKJyUmgE314e4ZyUnLkHw" alt=""><figcaption></figcaption></figure>
12. Paste your Personal Access Token and Base URL and click on Integrate GitLab.

    <figure><img src="https://lh5.googleusercontent.com/uiW1_fV35ZKCu1d6Xlr_m3RhedhYYr-h52jqm9HhjX5u9CqTX3LMqHxbqB5RMSdMT0Zr5lhq1zc4HtiWaIfl7MYy4vP7rvCDYgCut44PDPwru19XU4L3t6D_9WA0BWsCKVX-hSpro6RB71o7yJYbmJU" alt=""><figcaption></figcaption></figure>
13. You have now successfully integrated GitLab into DevDynamics.

    <figure><img src="https://lh5.googleusercontent.com/SScS8atHDpvvTbwDjI04Vt2iP93y6mFZbdzFpsX_jrFCDjsFnQGP3YZFtClLi4NYhTK3quTgCvky3WiNBpuDFdD-Z80U-Ng-Mhkg-kJESpHlbxY0rTG2f-Klg5_ns3H_0caVYKDJoQcNhIhgxPrVyeM" alt=""><figcaption></figcaption></figure>
