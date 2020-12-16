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


part1.2

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


Part1.3


import React from 'react'
import ReactDOM from 'react-dom'
const Header = (props)=>{
  console.log(props)
  return(
    <div>
<h1>{props.course}</h1>

    </div>
  )
}


const Total = (props) =>{
  console.log(props)
  return(
    <div>
    <p>Number of exercises {props.exercises1 + props.exercises2 + props.exercises3}</p>

    </div>
  )
}


    const Parts = (props) =>{
      console.log(props)
        return(
            <div>
            <p> {props.name}  {props.exercises}</p>
            </div>
        )
    }
    const Content=()=> {
  
     
      console.log()
      const part1 = {
        name: 'Fundamentals of React',
        exercises: 10,
   
      }
      
      const part2 = {
        name: 'Using props to pass data',
        exercises: 7
      }
      const part3 = {
        name: 'State of a component',
        exercises: 14
      }
  return(
  
    <div>
     <Parts name={part1.name} exercises={part1.exercises} />
      <Parts name={part2.name} exercises={part2.exercises} />
      <Parts name={part3.name} exercises={part3.exercises} />
    </div>
  )
}

const App = () => {
  const course = 'Half Stack application development'
  const part1 = {
    name: 'Fundamentals of React',
    exercises: 10
  }
  const part2 = {
    name: 'Using props to pass data',
    exercises: 7
  }
  const part3 = {
    name: 'State of a component',
    exercises: 14
  }

  return (
    <div>
      
       <Header course={course}/>
       
       
       <Content/>
       
       
    <Total exercises1={part1.exercises} exercises2={part2.exercises} exercises3={part3.exercises} />
       
    
    </div>
  )
}

ReactDOM.render(<App />, document.getElementById('root'))

part1.4



import React from 'react'
import ReactDOM from 'react-dom'
const Header = (props)=>{
  console.log(props)
  return(
    <div>
<h1>{props.course}</h1>

    </div>
  )
}


const Total = (props) =>{
  console.log(props)
  return(
    <div>
    <p>Number of exercises {props.exercises1 + props.exercises2 + props.exercises3}</p>

    </div>
  )
}


    const Parts = (props) =>{
      console.log(props)
        return(
            <div>
            <p> {props.name}  {props.exercises}</p>
            </div>
        )
    }
    const Content=()=> {
  
     
      console.log()
      const course = 'Half Stack application development'
  const parts = [
    {
      name: 'Fundamentals of React',
      exercises: 10
    },
    {
      name: 'Using props to pass data',
      exercises: 7
    },
    {
      name: 'State of a component',
      exercises: 14
    }
  ]

  return(
  
    <div>
     <Parts name={parts[0].name} exercises={parts[0].exercises} />
      <Parts name={parts[1].name} exercises={parts[1].exercises} />
      <Parts name={parts[2].name} exercises={parts[2].exercises} />
    </div>
  )
}

const App = () => {
  const course = 'Half Stack application development'
  const parts = [
    {
      name: 'Fundamentals of React',
      exercises: 10
    },
    {
      name: 'Using props to pass data',
      exercises: 7
    },
    {
      name: 'State of a component',
      exercises: 14
    }
  ]


  return (
    <div>
      
       <Header course={course}/>
       
       
       <Content/>
       
       
    <Total exercises1={parts[0].exercises} exercises2={parts[1].exercises} exercises3={parts[2].exercises} />
       
    
    </div>
  )
}

ReactDOM.render(<App />, document.getElementById('root'))

Part1.5


import React from 'react'
import ReactDOM from 'react-dom'
const Header = (props)=>{
  console.log(props)
  return(
    <div>
<h1>{props.course.name}</h1>

    </div>
  )
}


const Total = (props) =>{
  console.log(props)
  return(
    <div>
    <p>Number of exercises {props.exercises1 + props.exercises2 + props.exercises3}</p>

    </div>
  )
}


    const Parts = (props) =>{
      console.log(props)
        return(
            <div>
            <p> {props.name}  {props.exercises}</p>
            </div>
        )
    }
    const Content=()=> {
  
     
      console.log()
      const course = {
        name: 'Half Stack application development',
        parts: [
          {
            name: 'Fundamentals of React',
            exercises: 10
          },
          {
            name: 'Using props to pass data',
            exercises: 7
          },
          {
            name: 'State of a component',
            exercises: 14
          }
        ]
      }

  return(
  
    <div>
     <Parts name={course.parts[0].name} exercises={course.parts[0].exercises} />
      <Parts name={course.parts[1].name} exercises={course.parts[1].exercises} />
      <Parts name={course.parts[2].name} exercises={course.parts[2].exercises} />
    </div>
  )
}

const App = () => {
  
  const course = {
    name: 'Half Stack application development',
    parts: [
      {
        name: 'Fundamentals of React',
        exercises: 10
      },
      {
        name: 'Using props to pass data',
        exercises: 7
      },
      {
        name: 'State of a component',
        exercises: 14
      }
    ]
  }
  return (
    <div>
      
       <Header course={course}/>
       
       
       <Content/>
       
       
    <Total exercises1={course.parts[0].exercises} exercises2={course.parts[1].exercises} exercises3={course.parts[2].exercises} />
       
    
    </div>
  )
}

ReactDOM.render(<App />, document.getElementById('root'))

part1.6

import React, { useState } from 'react'
import ReactDOM from 'react-dom'

const App = () => {
  // save clicks of each button to its own state
  const [good, setGood] = useState(0)
  const [neutral, setNeutral] = useState(0)
  const [bad, setBad] = useState(0)

  return (
    <div>
     <h1>give feed back</h1> 
     <button onClick={()=>setGood(good+1)}> good </button>
     <button onClick={()=>setNeutral(neutral+1)}> neutral </button>
     <button onClick ={()=>setBad(bad+1)}>bad</button>
     <h1>statistics</h1>
     <div>good {good}</div>
     <div>neutral {neutral}</div>
     <div>bad {bad}</div>
    </div>
  )
}

ReactDOM.render(<App />, 
  document.getElementById('root'))
  
  part1.7
  
  import React, { useState } from 'react'
import ReactDOM from 'react-dom'

const App = () => {
  // save clicks of each button to its own state
  const [good, setGood] = useState(0)
  const [neutral, setNeutral] = useState(0)
  const [bad, setBad] = useState(0)
  const [all,setAll] = useState(0)
  const [average ,setAverage] = useState(0)
  
  const handleGoodClick =() =>{
    setAll(all+1)
  setGood(good+1)
  setAverage(average+1)
}
  const handleNeutralClick = () => {
    setAll(all+1)
    setNeutral(neutral+1)
    
  }
const handleBadClick =() => {
setAll(all+1)
setBad(bad+1)
setAverage(average-1)
}

  return (
    <div>
     <h1>give feed back</h1> 
     <button onClick={handleGoodClick}> good </button>
     <button onClick={handleNeutralClick}>neutral </button>
     <button onClick ={handleBadClick}>bad</button>
    
     <h1>statistics</h1>
     <div>good {good}</div>
     <div>neutral {neutral}</div>
     <div>bad {bad}</div>
     <div> all {all} </div>
     <div>average  {average/all} </div>
     <div> positive {good/all*100} % </div>
    </div>
     
  )
}

ReactDOM.render(<App />, 
  document.getElementById('root'))
  
  part1.8
  import React, { useState } from 'react'
import ReactDOM from 'react-dom'

  
const Statistics = (props) => {
  
    
  return (
    <div> 
   <div> good {props.good} </div>
    <div> neutral {props.neutral}</div>
    <div>bad {props.bad}</div>
    <div> all {props.all} </div>
     <div>average  {props.average/props.all} </div>
     <div> positive {props.good/props.all*100} % </div>
     
    </div>
  )

}
const App = () => {
  // save clicks of each button to its own state
  const [good, setGood] = useState(0)
  const [neutral, setNeutral] = useState(0)
  const [bad, setBad] = useState(0)
  const [all,setAll] = useState(0)
  const [average ,setAverage] = useState(0)
  
  const handleGoodClick =() =>{
    setAll(all+1)
  setGood(good+1)
  setAverage(average+1)
}
  const handleNeutralClick = () => {
    setAll(all+1)
    setNeutral(neutral+1)
    
  }
const handleBadClick =() => {
setAll(all+1)
setBad(bad+1)
setAverage(average-1)
}

  return (
    <div>
     <h1>give feed back</h1> 
     <button onClick={handleGoodClick}> good </button>
     <button onClick={handleNeutralClick}>neutral </button>
     <button onClick ={handleBadClick}>bad</button>
    
     <h1>statistics</h1>
     <Statistics good = {good}
      neutral = {neutral}
     bad = {bad}
     all = {all} 
      average = {average}
      positive = {good/all*100}/>
      
    </div>
     
  )
}

ReactDOM.render(<App />, 
  document.getElementById('root'))
  
  part1.9
  
  import React, { useState } from 'react'
import ReactDOM from 'react-dom'

  
const Statistics = (props) => {
  
    if(props.all===0) {
      return(
        <div> No feedback given</div>
      )
    }
  return (
    <div> 
   <div> good {props.good} </div>
    <div> neutral {props.neutral}</div>
    <div>bad {props.bad}</div>
    <div> all {props.all} </div>
     <div>average  {props.average/props.all} </div>
     <div> positive {props.good/props.all*100} % </div>
     
    </div>
  )

}
const App = () => {
  // save clicks of each button to its own state
  const [good, setGood] = useState(0)
  const [neutral, setNeutral] = useState(0)
  const [bad, setBad] = useState(0)
  const [all,setAll] = useState(0)
  const [average ,setAverage] = useState(0)
  
  const handleGoodClick =() =>{
    setAll(all+1)
  setGood(good+1)
  setAverage(average+1)
}
  const handleNeutralClick = () => {
    setAll(all+1)
    setNeutral(neutral+1)
    
  }
const handleBadClick =() => {
setAll(all+1)
setBad(bad+1)
setAverage(average-1)
}

  return (
    <div>
     <h1>give feed back</h1> 
     <button onClick={handleGoodClick}> good </button>
     <button onClick={handleNeutralClick}>neutral </button>
     <button onClick ={handleBadClick}>bad</button>
    
     <h1>statistics</h1>
     <Statistics good = {good}
      neutral = {neutral}
     bad = {bad}
     all = {all} 
      average = {average}
      positive = {good/all*100}/>
      
    </div>
     
  )
}

ReactDOM.render(<App />, 
  document.getElementById('root'))
  
  part1.10
  
  import React, { useState } from "react";
import ReactDOM from "react-dom";

const Statistic = (props) => {
  return (
    <div>
      {props.text} {props.value}
    </div>
  );
};

const Statistics = (props) => {
  if (props.all === 0) {
    return <div> No feedback given</div>;
  }
  return (
    <div>
      <Statistic text="good" good value={props.good} />
      <Statistic text="neutral" value={props.neutral} />
      <Statistic text="bad" value={props.bad} />
      <Statistic text="all" value={props.all} />
      <Statistic text="average" value={props.average / props.all} />
      <Statistic text="positive" value={(props.good / props.all) * 100 + "%"} />
    </div>
  );
};

const Button = ({ onClick, text }) => <button onClick={onClick}>{text}</button>;
const App = () => {
  // save clicks of each button to its own state
  const [good, setGood] = useState(0);
  const [neutral, setNeutral] = useState(0);
  const [bad, setBad] = useState(0);
  const [all, setAll] = useState(0);
  const [average, setAverage] = useState(0);

  const handleGoodClick = () => {
    setAll(all + 1);
    setGood(good + 1);
    setAverage(average + 1);
  };
  const handleNeutralClick = () => {
    setAll(all + 1);
    setNeutral(neutral + 1);
  };

  const handleBadClick = () => {
    setAll(all + 1);
    setBad(bad + 1);
    setAverage(average - 1);
  };

  return (
    <div>
      <h1>give feed back</h1>
      <Button onClick={handleGoodClick} text="good" />
      <Button onClick={handleNeutralClick} text="neutral" />
      <Button onClick={handleBadClick} text="bad" />

      <h1>statistics</h1>
      <Statistics
        good={good}
        neutral={neutral}
        bad={bad}
        all={all}
        average={average}
        positive={(good / all) * 100}
      />
    </div>
  );
};

ReactDOM.render(<App />, document.getElementById("root"));

part1.12

import React, { useState } from 'react'
import ReactDOM from 'react-dom'

const App = (props) => {
  const [selected, setSelected] = useState(0)

  
     
    
  return (
    <div>
      {props.anecdotes[selected]}
      <div>
      <button onClick ={()=>setSelected (Math.floor(Math.random()*7))}> next anecdote</button>
    </div>
    </div>
  )
}

const anecdotes = [
  'If it hurts, do it more often',
  'Adding manpower to a late software project makes it later!',
  'The first 90 percent of the code accounts for the first 90 percent of the development time...The remaining 10 percent of the code accounts for the other 90 percent of the development time.',
  'Any fool can write code that a computer can understand. Good programmers write code that humans can understand.',
  'Premature optimization is the root of all evil.',
  'Debugging is twice as hard as writing the code in the first place. Therefore, if you write the code as cleverly as possible, you are, by definition, not smart enough to debug it.'
]

ReactDOM.render(
  <App anecdotes={anecdotes} />,
  
  document.getElementById('root')
)

  
  
