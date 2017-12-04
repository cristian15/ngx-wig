ngx-Wig
=====

## Dependencies

*it's only Angular! No jQuery or other WYSIWYG monsters*


## Installation

ngx-wig could be simply installed via npm:

    npm install ngx-wig --save

### Important note:

The last version on ngx-wig that was built for Angular 4.x is 0.3.6.
Any higher version may be not fully compatible with Angular version lower than 5.0.0.


## Usage

First, import the ngx-wig to your module:

    import {Ng2WigModule} from 'ngx-wig';

    @NgModule({
      imports: [ Ng2WigModule]
    });


it's just attribute directive for textarea:

    <ng2wig [content]="text1"></ng2wig>



## Examples

### Quick start

    <ng2wig [content]="text1"></ng2wig>

### Placeholder

    <ng2wig  [content]="text1" [placeholder]="'Enter instructions here.'"></ng2wig>

### ngModel sync

    <ng2wig [content]="text1"></ng2wig>
    <ng2wig [content]="text1"></ng2wig>

### Set buttons

    <ng2wig  [content]="text1" [buttons]="formats, bold, italic"></ng2wig>


### onContentChange Hook

        <ng2wig [content]="text1" (contentChange)="update($event)"></ng2wig>


## Contribution (Development Setup)

    npm install
    npm start


