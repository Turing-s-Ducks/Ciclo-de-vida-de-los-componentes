# Ciclo-de-vida-de-los-componentes
Ciclo de vida de los componentes en JS .

``` Typescript 
// importamos las diferentes fases del ciclo de vida de los componentes
import { Component, OnInit, OnChanges, DoCheck, AfterContentInit, AfterContentChecked, AfterViewInit, AfterViewChecked, OnDestroy } from '@angular/core';

@Component({
  selector: 'app-fases',
  templateUrl: './fases.component.html',
})

export class fasesComponent implements OnInit ,OnChanges,DoCheck,AfterContentInit,AfterContentChecked,AfterViewInit,AfterViewChecked,OnDestroy{

  constructor() { }

  ngOnInit() {
    console.log('ngOnInit');
  }
  ngOnChanges(){
    console.log('ngOnChanges');
  }
  ngDoCheck(){
    console.log('ngDoCheck');
    
  }
  ngAfterContentInit(){
    console.log('ngAfterContentInit');
    
  }
  ngAfterContentChecked(){
    console.log('ngAfterContentChecked');
    
  }
  ngAfterViewInit(){
    console.log('ngAfterViewInit');
    
  }
  ngAfterViewChecked(){
    console.log('ngAfterViewChecked');
    
  }
  ngOnDestroy(){
    console.log('ngOnDestroy');
    
  }
}
````
