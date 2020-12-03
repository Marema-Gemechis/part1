# Full-stack-exercises

Part 1.1

import React from 'react'
import ReactDOM from 'react-dom'
const Header = (props)=>{
  return(
    <div>
<h1>{props.course}</h1>

    </div>
  )
}
const Content = (props) =>{

  return(
    <div>
<p> {props.part1}  {props.exercise1}</p>
<p>{props.part2} {props.exercise2}</p>
<p>{props.part3} {props.exercises3}</p>
    </div>
  )
}
const Total = (props) =>{
  return(
    <div>
    <p>Number of exercises {props.exercises1 + props.exercises2 + props.exercises3}</p>

    </div>
  )
}

const App = () => {
  const course = 'Half Stack application development'
  const part1 = 'Fundamentals of React'
  const exercises1 = 10
  const part2 = 'Using props to pass data'
  const exercises2 = 7
  const part3 = 'State of a component'
  const exercises3 = 14

  return (
    <div>
       <Header course={course}/>
       <Content part1= {part1} exercise1={exercises1}/>
    <Content part2={part2} exercise2={exercises2}/>
    <Content part3= {part3} exercise3={exercises3}/>
    <Total exercises1={exercises1} exercises2={exercises2} exercises3={exercises3} />
       
    </div>
  )
}

ReactDOM.render(<App />, document.getElementById('root'))


PART1.2
import React from 'react'
import ReactDOM from 'react-dom'
const Header = (props)=>{
  return(
    <div>
<h1>{props.course}</h1>

    </div>
  )
}


const Total = (props) =>{
  return(
    <div>
    <p>Number of exercises {props.exercises1 + props.exercises2 + props.exercises3}</p>

    </div>
  )
}


    const Part = (props) =>{
        return(
            <div>
            <p> {props.part}  {props.exercises}</p>
            </div>
        )
    }
    const Content = () =>{
        const part1 = 'Fundamentals of React'
  const exercises1 = 10
  const part2 = 'Using props to pass data'
  const exercises2 = 7
  const part3 = 'State of a component'
  const exercises3 = 14

    return(
      <div>
      <Part part={part1} exercises={exercises1}/> 
      <Part part={part2} exercises={exercises2}/>
      <Part part={part3} exercises={exercises3}/>
      </div>
    )
  }

const App = () => {
  const course = 'Half Stack application development'
  const exercises1 = 10
  const exercises2 = 7
  const exercises3 = 14

  return (
    <div>
       <Header course={course}/>
       
        <Content/>

       
       
    <Total exercises1={exercises1} exercises2={exercises2} exercises3={exercises3} />
       
    </div>
  )
}

ReactDOM.render(<App />, document.getElementById('root'))
