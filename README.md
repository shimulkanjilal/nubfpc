# NUB Film & Photography Club (NUBFPC) Website

The official website of the **NUB Film & Photography Club**, Northern University Bangladesh. It is a single-file static site (`nub_film_photography_club_final_v82.html`) with no build step and no backend required.

## Features

- **Public pages and sections**: About Us, Announcements, Upcoming Events, Showcase / Photo of the Moment, Films, Current and Past Events, Team, Mentors, Members, Blood Donor Directory, Join Us (recruitment), University info and contact, Photo Contest, Results, Sponsors
- **Admin dashboard** (fullscreen, sidebar layout) for managing content, logos, photos, team, events, announcements, contests and results
- **Certificate Maker** and **Event ID Card / Badge Maker** (admin only), with QR codes via `qrcode-generator`
- **Image uploads** through Cloudinary (unsigned preset)
- **Responsive design** built with Bootstrap 5 and Bootstrap Icons

## Tech stack

| Area | Details |
| --- | --- |
| Markup, style, logic | Plain HTML, CSS, vanilla JavaScript (single file) |
| UI | Bootstrap and Bootstrap Icons (via jsDelivr CDN) |
| Fonts | Google Fonts |
| QR codes | qrcode-generator 1.4.4 (MIT, inlined) |
| Image hosting | Cloudinary |
| Data storage | Browser `localStorage` (local mode) |

## Configuration

All editable content lives in the `CONFIG` object near the top of the main script:

| Key | Purpose |
| --- | --- |
| `firebase` | Left empty (Firebase removed) |
| `cloudinary` | `cloudName`, `uploadPreset` (must be **unsigned**), `folder` |
| `links` | Facebook, Instagram, LinkedIn URLs |
| `contact` | Email, address, map query |
| `recruitment` | Join section title, subtitle, perks, optional `formUrl` |
| `announcements` | Notices with title, text, date, expiry, tag, link |
| `about` / `aboutUs` | About text, mission, vision, activities, benefits |
| `events` | Event list. Status (ongoing, upcoming, past) is automatic from dates; add `status:"past"` to force it |
| `activities` | Partnerships and organised programs |

Most of this content can also be edited from the Admin dashboard without touching the code.

## Contact

- Email: nubfpc@nub.ac.bd
- Facebook: https://www.facebook.com/share/1FmP15hu3Y/
- Instagram: https://www.instagram.com/nubfpc
- LinkedIn: https://www.linkedin.com/company/nubfpc/
- Address: Northern University Bangladesh, Ashkona, Dakshin Khan, Dhaka-1230, Bangladesh

## License

Content, logos and photos belong to NUB Film & Photography Club and their respective creators. Third-party libraries keep their own licenses.
