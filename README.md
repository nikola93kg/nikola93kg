- š Hi, Iām @nikola93kg
- š Iām interested in Frontend Development
- š± Iām currently learning advanced ReactJS
- šļø Iām looking to collaborate on interesting projects
- š« Reach me at https://nikola93kg.github.io/

<!---
nikola93kg/nikola93kg is a āØ special āØ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->


import React from 'react';

function ApplyForAJob() {

    const jobApply = [{
      id: 0,
      greet: 'Hello',
      bodyMsg: 'I want to apply as a front-end developer. You can find more info about me at my portfolio website:',
      url: 'https://nikola93kg.github.io/'
    }]

    const containerStyle = {
      display: 'grid',
      placeItems: 'center',
      height: '100vh',
      background: 'linear-gradient(120deg, #0f73e5df, #fff)',
      color: 'white',
      fontSize: '1.5em'
    }
    const linkStyle = {
      color: '#0f72e5',
      textDecoration: 'none',
      fontSize: '1.2em'
    }

    return (
      <div style={containerStyle}>
        {
          jobApply.map(job => {
            return (
              <div className='container__body' key={job.id}>
                <h1>{job.greet}</h1>
                <p>{job.bodyMsg}</p>
                <a href={job.url} style={linkStyle} target="_blank">https://nikola93kg.github.io/</a>
              </div>
            )
          })
        }
      </div >
    )
  }

export default ApplyForAJob;

![Screenshot_2](https://user-images.githubusercontent.com/53098565/172687156-46431b63-ce4b-441b-84fc-cee7817fd50f.png)


