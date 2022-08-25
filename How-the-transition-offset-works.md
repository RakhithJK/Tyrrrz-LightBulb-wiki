Transition offset allows you to specify how early or late the transitions start, relative to sunrise and sunset.
It's best to understand how it works by looking at some examples.
For the purpose of demonstration, let's assume that sunset takes place at 5:00 AM, sunrise at 7:00 PM, and transition duration is set to 40 minutes.

- **0% offset** (default)

  - Day-time transition starts before sunrise at 4:20 AM and ends precisely at sunrise at 5:00 AM.
  - Night-time transition starts precisely at sunset at 7:00 PM and ends after sunset at 7:40 PM.

- **25% offset**

  - Day-time transition starts 75% before sunrise at 4:30 AM and ends 25% after sunrise at 5:10 AM.
  - Night-time transition starts 25% before sunset at 6:50 PM and ends 75% after sunset at 7:30 PM.

- **50% offset**

  - Day-time transition starts halfway before sunrise at 4:40 AM and ends halfway after sunrise at 5:20 AM.
  - Night-time transition starts halfway before sunset at 6:40 PM and ends halfway after sunset at 7:20 PM.

- **75% offset**

  - Day-time transition starts 25% before sunrise at 4:50 AM and ends 75% after sunrise at 5:30 AM.
  - Night-time transition starts 75% before sunset at 6:30 PM and ends 25% after sunset at 7:10 PM.

- **100% offset**

  - Day-time transition starts precisely at sunrise at 5:00 AM and ends after sunrise at 5:40 AM.
  - Night-time transition starts before sunset at 7:00 PM and ends precisely at sunset at 7:40 PM.

Depending on factors such as window angle, elevation, building density, presence of trees or mountains, etc., adjusting this offset may help bring your monitor's gamma cycle more in line with how the solar cycle is perceived in your environment.