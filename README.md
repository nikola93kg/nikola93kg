- 👋 Hi, I’m @nikola93kg
- 👀 I’m interested in Frontend Development
- 🌱 I’m currently learning advanced ReactJS
- 💞️ I’m looking to collaborate on interesting projects
- 📫 Reach me at https://nikola93kg.github.io/

<!---
nikola93kg/nikola93kg is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->


import React from 'react'

function ApplyForJob() {

    const jobApply = [{
        id: 0,
        greet: 'Hello',
        bodyMsg: 'I want to apply as a front-end developer. You can find more info about me at my portfolio website',
        url: 'https://nikola93kg.github.io/'
    }]

    return (
        <>
            {
                jobApply.map(job => {
                    return (
                        <div className='container' key={job.id}>
                            <h1>{job.greet}</h1>
                            <p>{job.bodyMsg}</p>
                            <a href={job.url} target="_blank">portfolio website</a>
                        </div>
                    )
                })
            }
        </>
    )
}

export default ApplyForJob
