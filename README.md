# CSE610 Mobile Systems and Edge Intelligence — Fall 2026

Course website for CSE610 at the University at Buffalo, SUNY.

Live site: https://xieyaxiongfly.github.io/CSE610_Mobile/

## Course Information

**Instructor:** Yaxiong Xie
**Email:** yaxiongx@buffalo.edu
**Office:** Davis Hall 321
**Office Hours:** By appointment — please email to schedule

**Lecture Time:** TBA
**Location:** TBA
**Semester:** Fall 2026

## Course Description

This course examines how modern mobile and embedded systems sense, communicate, and compute, and how machine intelligence is pushed from the cloud to the edge and onto the device itself. Topics span mobile and wireless sensing, mobile platform and OS architecture, energy- and latency-aware system design, edge/cloud offloading, on-device inference, model compression and acceleration, and privacy in mobile and edge deployments. The course is research-oriented: students read and present recent papers from venues such as MobiCom, MobiSys, SenSys, NSDI, and MLSys, and complete a semester-long project.

## Website Features

- 📅 **Smart Schedule System**: automatically generates class dates from the semester start date and configured class days
- 📚 **Course Materials**: organized lectures, assignments, and project information
- 👥 **Staff Information**: instructor and TA profiles
- 📱 **Responsive Design**: works on desktop and mobile
- 🎛️ **Web Dashboard**: Flask interface for editing course content without touching files by hand

## Repository Layout

| Path | Purpose |
| --- | --- |
| `_config.yml` | Course name, description, semester, `baseurl` |
| `_data/course_schedule.yml` | Semester dates, class days, holidays, lecture sequence |
| `_data/home_modules.yml` | Blocks rendered on the home page |
| `_data/people.yml` | Instructor and TA entries |
| `_data/assignments.yml` | Assignment policy text and assignment list |
| `_data/textbooks.yml` | Textbooks shown on the Materials page |
| `_lectures/`, `_assignments/`, `_events/`, `_announcements/` | Jekyll collections |
| `static_files/uploads/` | Slides, handouts, and other uploaded PDFs |
| `dashboard/` | Flask content-management dashboard (not published) |

See `README_SCHEDULE.md` and `SCHEDULE_CONFIG_EXAMPLES.md` for how the schedule generator works.

## Local Development

```bash
bundle install
bundle exec jekyll serve
# then open http://localhost:4000/CSE610_Mobile/
```

Or use the helper scripts:

```bash
./dashboard/start-site.sh   # Jekyll preview
./dashboard/start.sh        # content dashboard
```

## Deployment

The site is published with GitHub Pages from this repository. `baseurl` is set to `/CSE610_Mobile`; if the repository is renamed, update `baseurl` in `_config.yml` to match.
